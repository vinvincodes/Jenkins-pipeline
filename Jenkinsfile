pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building..."
            }
            post{
                success{
                    mail to:"vinajoit@gmail.com",
                    subject:"Build Status Email",
                    body:"Build was successful!"
                }
            }
        }
    }

    stages {
        stage('Build') {
            steps {
                echo "Building..."
            }
        }
    }

     stages {
        stage('Test') {
            steps {
                echo "Testing..."
            }
        }
    }

     stages {
        stage('Deploy') {
            steps {
                echo "Deploying..."
            }
        }
    }

     stages {
        stage('Complete') {
            steps {
                echo "Completed..."
            }
        }
    }
}
