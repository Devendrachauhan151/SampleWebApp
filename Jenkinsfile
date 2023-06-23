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
                sh 'cp -R /var/lib/jenkins/workspace/demo/Jenkinsfile /var/lib/jenkins/workspace/demo/TestCalculator_JUnitResult.txt.txt /var/lib/jenkins/workspace/demo/WebContent /var/lib/jenkins/workspace/demo/build /var/lib/jenkins/workspace/demo/build.xml /var/lib/jenkins/workspace/demo/checkstyle_errors.xml /var/lib/jenkins/workspace/demo/index.html /var/lib/jenkins/workspace/demo/src /var/lib/jenkins/workspace/demo/sun_checks.xml /var/lib/jenkins/workspace/demo/testing /var/www/html/'
            }
        }
    }
}
