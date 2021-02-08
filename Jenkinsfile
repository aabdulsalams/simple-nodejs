pipeline {

    agent any

    stages {
        
        stage("build") {
            
            steps{
                echo 'building the application'
                nodejs('basic-nodejs-15.8.0') {
                    sh 'npm install'
                }
            }
        }

        stage("test") {
            
            steps{
                echo 'testing the application'
                nodejs('basic-nodejs-15.8.0') {
                    sh 'pm2 start app.js'
                }
            }
        }

        stage("deploy") {
            
            steps{
                echo 'deploying the application'
            }
        }

    }
}