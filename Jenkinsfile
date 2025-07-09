pipeline {
    agent any
    
    environment {
        DEPLOY_TO = 'Production'
    }
    stages {
        stage('ProdDeploy'){
        when {
            environment name: 'DEPLOY_TO', value: 'Production'
        }
        steps{
            echo "deployment is sucess"
        }
    }
}
            
