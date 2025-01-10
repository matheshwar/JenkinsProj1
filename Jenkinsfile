pipeline {
    agent any

    stages {
        stage('Install pip') {
            steps {
                sh 'sudo apt-get update'
                sh 'sudo apt-get install python3-pip -y'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'pip3 install -r requirements.txt'
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
        stage('Deploy Application') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
