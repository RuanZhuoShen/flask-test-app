pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Test') {
            steps {
                echo 'Checking file exists...'
                sh 'ls -la index.html'
            }
        }
        stage('Deploy') {
            steps {
                sh 'bash deploy.sh'
            }
        }
    }
}
