pipeline {
    // don't use 'agent any'
    // 'agent none' allows the job to continue on the same node
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

        stage('Greetings') {
            steps {
                script {
                    sh "echo Hello $MY_ENV"
                    sh "echo GIT_COMMIT=$GIT_COMMIT"
                }
            }
        }
         
    }
}