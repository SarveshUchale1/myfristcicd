pipeline {
    agent any

    tools {
        nodejs 'node20'  // 👈 match the name you gave in Global Tool Configuration
    }

    stages {
        stage('Build') {
            steps {
                echo '📦 Building the project...'
               
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
               
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the project...'
                
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
