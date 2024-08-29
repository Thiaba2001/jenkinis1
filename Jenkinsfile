pipeline {
    agent any
    triggers{
        cron('* * * * *')
    }

    stages{
        stage{
            steps{
                echo build!
            }
        }
    }
}