pipeline{
    agent any 
    tools {
        maven 'maven-3.8.8'
    }
    stages {
        stage('Build') {
            steps {
                echo "*****I want to build know*****"
            } 
        }
        stage('Test') {
            steps{
                echo"****I want to test my application****"
            }
        }
            stage('Deploy') {
                steps{
                    echo"****I want to deploy my application****"
                }

            }
        }
}
