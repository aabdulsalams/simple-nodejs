pipeline {

    agent any

    stages {
        
        stage("build") {
            
            steps{
                echo 'building the application'
                sh 'npm install'
            }
        }

        stage("test") {
            
            steps{
                echo 'testing the application'
                sh 'pm2 start app.js'
            }
        }

        stage("deploy") {
            
            steps{
                echo 'deploying the application'
            }
        }

    }
}