pipeline {
    agent any
    environment {
        DEPLOY_TO = 'Production'
    }
    stages {
        stage('Deploytoproduction')
        when {
            environment name: DEPLOY_TO, Value: Production
        }
        steps{
            echo "deployment is sucess"
        }
    }
}
            
