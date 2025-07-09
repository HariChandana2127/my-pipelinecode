pipeline{
    agent any
    environment{
        GITHUB_CREDS =credintials ('github')
        stages{
            stage('Build'){
                steps{
                    echo "my git hub credintials ***"
                    echo "my username = $ {GITHUB_CREDS_USR}"
                    echo "my password = $ {GITHUB_CREDS_PSW}"
                }
            }
        }  
                
}
