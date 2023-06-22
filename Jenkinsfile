pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/Devendrachauhan151/SampleWebApp.git'
            }
         stage('Deploy to Nginx') {
            steps {
                // Deploy the application to the production environment
                sh 'cp -R /* /var/www/html'
            }
        }
    }
}
