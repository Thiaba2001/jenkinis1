pipeline {
    agent any 
    tools {
        gradle 'gradle8.10'
    }

    stages {
        stage('build'){
            steps{
                sh 'gradle -v'
            }
        }
        
}

}