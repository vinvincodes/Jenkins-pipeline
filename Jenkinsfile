pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building the code..."
            }
            post {
                success {
                    mail to: "vinajoit@gmail.com",
                    subject: "Build Status Email",
                    body: "Build was successful!"
                }
            }
        }

        stage('Unit and Integration Test') {
            steps {
                echo "Running unit and integration tests..."
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Analysing the code..."
            }
        }

        stage('Security Scan') {
            steps {
                echo "Performing security scan..."
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploying to Staging environment..."
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on staging..."
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying to production environment..."
            }
        }
    }
}
