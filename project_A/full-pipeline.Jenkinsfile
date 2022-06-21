pipeline {
    // don't use 'agent any'
    // 'agent none' allows the job to continue on the same node with the same files
    agent none 

    environment {
    MY_ENV = "Devops"
    GIT_COMMIT= "${COMMIT}"
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
                     sh "echo Environment passed: GIT_COMMIT=$GIT_COMMIT"
                }
            }
        }
         
    }
}