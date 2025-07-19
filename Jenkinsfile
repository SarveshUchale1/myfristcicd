pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '📦 Installing dependencies...'
                bat 'npm install docker'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                bat 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Starting app...'
                bat 'start /b node app.js'
            }
        }
    }

    post {
        success {
            echo '✅ Build and deploy completed!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
