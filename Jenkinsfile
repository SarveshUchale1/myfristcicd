pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '📦 Building the project...'
                // For Node.js example
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                // For demo, pretend test passes
                sh 'node test.js'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the project...'
                // Just a demo deploy (you can expand later)
                sh 'echo "Deployment complete"'
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
