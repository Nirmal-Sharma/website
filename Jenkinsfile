pipeline{
    agent any
    environment{
        staging_server="10.1.1.103"
    }
    stages{
        stage('Deploy to Remote-Server'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/coffe/'
                
            }
        }
    }
}
