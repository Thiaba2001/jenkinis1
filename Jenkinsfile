pipeline {
    agent any

    stages{
        stage('build'){
            steps{
                echo 'build !'
            }    
        }

        stage('deployment production') {
            input {
                message 'voulez-vous déployer en production ?'
                ok 'déployer !'
                submitter 'admin,devops'
                submitterParameter 'USER_SUBMIT'
                parameters{
                    string(name: 'VERSION',defaultValue: 'latest',description: 'une version')

                }
            }
                steps {
                    echo "user: ${USER_SUBMIT}"
                    echo "version: ${VERSION}"
                    echo 'deploy!'
                }

            }
        }
    }
