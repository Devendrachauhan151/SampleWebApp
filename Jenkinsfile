pipeline {
    agent any

    stages {
        stage('Git checkout') {
            steps {
                git 'https://github.com/Devendrachauhan151/SampleWebApp.git'
            }
        }
        
        stage('Copy to Remote Nginx') {
            steps {
                ssh 'sudo scp -r /var/lib/jenkins/workspace/demo/testing.conf /etc/nginx/sites-enabled/'
                ssh 'sudo systemctl restart nginx'
                sh 'scp -r /var/lib/jenkins/workspace/demo/* /var/www/'
            }
        }
    }
}
