pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Building the code using Maven..."
                // Use Maven as a build automation tool as the example
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Running unit tests and integration tests..."
                // test automation tools such as: Selenium, Junit, Docker, etc.
            }

            post {
                success {
                    mail to: "vinajoit@gmail.com",
                    subject: "Unit and Integration Tests SUCCESSFULLY",
                    body: "Congrats! Unit and integration were successful!"
                }
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Analysing the code using PMD..."
                // Code analysis tool: PMD, CheckStyle, FindBugs, etc. 
            }
        }

        stage('Security Scan') {
            steps {
                echo "Performing security scan..."
            }
           

            post {
                success {
                    mail to: "vinajoit@gmail.com",
                    subject: "Security Scan SUCCESSFULLY",
                    body: "Congrats! Security Scan was successful!"
                }
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploying the application to a staging server..."
                // Deployment tool: e.g., AWS EC2 instance.
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on the staging environment..."
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying the application to a production server..."
                 // Deployment tool: e.g., AWS EC2 instance.
            }
        }

        stage('Completed') {
            steps {
                echo "Completed"
            }
            post {
                success {
                    mail to: "vinajoit@gmail.com",
                    subject: "Successfully and Completed!",
                    body: "Congrats! It's now successfully!"
                }
            }
        }

        
    }
}
