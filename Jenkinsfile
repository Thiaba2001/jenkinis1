pipeline {
    agent any 
    stages {
        stage('buid'){
            failFast true
            parallel{
                stage('build frotent'){
            steps{
                echo 'build!'
            }
        }
        stage('build backend'){
            steps{
                echo 'build backend!'
            }
        }

            }
        }
        stage('buid production'){
            steps{
                echo 'buikd production'
            }
        }
    }
}