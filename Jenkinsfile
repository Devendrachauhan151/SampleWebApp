pipeline {
    agent any

    stages {
        stage('Git checkout') {
            steps {
                git 'https://github.com/Devendrachauhan151/SampleWebApp.git'
            }
        }
        
        stage('Copy to Nginx path') {
            steps {
                sh 'cp -R /var/lib/jenkins/workspace/demo/* /var/www/html/'
                sh'sudo systemctl restart nginx '
            }
        }
    }
}
