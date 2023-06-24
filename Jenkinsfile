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
                sh 'scp -r $WORKSPACE/* $USER@$IP:$PATH'
            }
        }
    }
}
