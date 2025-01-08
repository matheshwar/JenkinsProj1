pipeline {
    agent any
    stages {
        stage('setupA') {
            steps {
                sh './install-dependencies.sh'
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
