pipeline{
    agent any
    environement{
        course="docker & k8s"
        name="hari"
    }
    stages{
        stage('Build'){
            environment{
                cloud="GCP"
            }
            steps{
                echo "welcome ${name}"
                echo "you enrolled in ${course}"
                echo "you certified in ${cloud}"
            }
        }
    }
}
