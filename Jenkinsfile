pipeline{
    agent any
    environment{
        staging_server="34.209.240.237"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE}${fil} root@${staging_server}:/var/www/html/${fil}'              
            }
        }
    }
}
