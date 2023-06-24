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
                sh 'scp -r /var/lib/jenkins/workspace/demo/* ubuntu@3.111.40.189:/var/www/html/'
            }
        }
    }
}
