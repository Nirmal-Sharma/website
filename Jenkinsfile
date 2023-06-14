pipeline{
    agent any
    environment{
        staging_server="35.90.7.13"
    }
    stages{
        stage('Deploy to Remote-Server'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                
            }
        }
    }
}
