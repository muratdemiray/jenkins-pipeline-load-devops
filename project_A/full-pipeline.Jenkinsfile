pipeline {
    agent none

    environment {
    MY_ENV = "Devops"
    }

    stages {     
        
        stage('List Files') {
            steps {
                script {
                    sh "ls -al"
                }
            }
        }

        stage('List Files') {
            steps {
                script {
                    sh "echo Hello $MY_ENV"
                }
            }
        }
         
    }
}