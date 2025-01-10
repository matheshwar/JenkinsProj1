pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install -r requirements.txt'
            }
        }
        stage('Build Application') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Test Application') {
            steps {
                sh 'npm run test'
            }
        }
    }
