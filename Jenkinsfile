pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                git credentialsId: 'git-test', url: 'https://github.com/Devendrachauhan151/SampleWebApp.git'
            }
        }
    }
}
