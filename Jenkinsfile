pipeline {
    agent any
    stages {
        stage('setup') {
            steps {
                bat 'npm run buildaa'
            }
        }
        stage('Install Dependencies') {
            steps {
                script {
                    // Ensure npm is installed
                    sh 'npm install'
                }
            }
        }
    }
    
}
