pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'github', usernameVariable: 'GITHUB_CREDS_USR', passwordVariable: 'GITHUB_CREDS_PSW')]) {
                    echo "My GitHub credentials:"
                    echo "Username: ${GITHUB_CREDS_USR}"
                    echo "Password: ${GITHUB_CREDS_PSW}"
                }
            }
        }
    }
}
