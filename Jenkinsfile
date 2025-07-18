pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '📦 Building the project...'
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                bat 'node test.js'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the project...'
                bat 'echo Deploy completed'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully.'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
