pipeline {
    agent any 
    stages {
        stage('buid and test'){
            matrix {
                axes {
                    axis{
                        name 'PLATEFORM'
                        value 'linus','macos','windows'
                    }
                    axis{
                        name 'BROWSER'
                        value 'firefox','chrome','safari'
                    }
                }
                stages{
                    stage('build'){
                        steps{
                            echo "construire pour ${PLATEFORM} . ${BROWSER}"
                        }
                    }
                    stage('test'){
                        steps{
                            echo "test pour ${PLATEFORME} .${BROWSER}"                      
                         }
                    }
                }
            }

        }
        stage('deployment production'){
            steps{
                echo 'deploys!'
            }
        }
        
}

}