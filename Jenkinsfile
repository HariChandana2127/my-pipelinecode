pipeline {
    agent any

    environment {
        DEPLOY_TO = 'Production'
    }

    stages {

        stage('Build') {
            steps {
                echo "***** I want to build now *****"

                // Credentials block inside build step
                withCredentials([usernamePassword(
                    credentialsId: 'github', 
                    usernameVariable: 'GITHUB_CREDS_USR', 
                    passwordVariable: 'GITHUB_CREDS_PSW')]) {

                    echo "My GitHub credentials:"
                    echo "Username: ${GITHUB_CREDS_USR}"
                    echo "Password: ${GITHUB_CREDS_PSW}"
                }
            }
        }

        stage('Test') {
            steps {
                echo "**** I want to test my application ****"
            }
        }

        stage('Deploy') {
            when {
                environment name: 'DEPLOY_TO', value: 'Production'
            }
            steps {
                echo "**** I want to deploy my application ****"
                echo "Deployment is successful"
            }
        }

    }
}
