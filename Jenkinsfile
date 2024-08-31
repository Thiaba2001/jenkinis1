pipeline {
    agent any 

    stages{
        stage('build'){
            steps{
                echo 'hello'
               
            }
        }

    post{
        success{
             emailext( to:'thiabadione@esp.sn' ,  body:'test body', subjec:'test subject')
        }
    }
    }

}