pipeline{
    agent any
    environment{
        staging_server="34.209.240.237"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'rsync -avzh ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                
            }
        }
    }
}
