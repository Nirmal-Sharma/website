pipeline{
    agent any
    environment{
        staging_server="34.219.52.20"
    }
    stages{
        stage('Deploy to Remote-Server'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                
            }
        }
    }
}
