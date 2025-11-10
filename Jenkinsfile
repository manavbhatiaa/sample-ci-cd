pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/manavbhatiaa/simple-cicd-demo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'bash build.sh'
            }
        }

        stage('Deploy (Demo)') {
            steps {
                echo 'Deploying build files (simulated)...'
                echo 'Deployment complete!'
            }
        }
    }

    post {
        success {
            echo "✅ CI/CD pipeline executed successfully!"
        }
        failure {
            echo "❌ Pipeline failed!"
        }
    }
}
