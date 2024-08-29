pipeline {
    agent any 
    stages {
        stage('buid and test'){
            matrix {
                axes {
                    axis{
                        name 'PLATEFORM'
                        values 'linus','macos','windows'
                    }
                    axis{
                        name 'BROWSER'
                        values 'firefox','chrome','safari'
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
                            echo "test pour ${PLATEFORM} . ${BROWSER}"                      
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