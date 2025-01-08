pipeline {
    agent any
    stages {
        stage('setup') {
            steps {
                bat 'npm run build'
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
