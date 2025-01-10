pipeline {
    agent any

    stages {
        stage('Build Applicatin') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test Application') {
            steps {
                sh 'npm run test'
            }
        }
        stage('Deploy Application') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
