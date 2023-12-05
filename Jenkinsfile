pipeline {
    agent any

    environment {
        // Define environment variables if needed
        EXAMPLE_VARIABLE = 'example_value'
    }

    stages {
        stage('HelloWorld') {
            steps {
                echo 'Hello, World!'
            }
        }

        stage('Build') {
            steps {
                // Your build steps go here
                echo 'Building...'
            }
        }

        stage('Test') {
            steps {
                // Use the docker.image directive to run steps inside a Docker container
                script {
                    def nodeImage = docker.image('node:16-alpine')
                    nodeImage.inside {
                        // Run commands inside the Docker container
                        sh 'node --version'
                        // Add additional test steps if needed
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                // Your deployment steps go here
                echo 'Deploying...'
            }
        }
    }

    post {
        always {
            // Actions to be performed regardless of the build result
            echo 'This will always be executed'
        }
        success {
            // Actions to be performed if the build succeeds
            echo 'Build succeeded'
            echo 'Happy coding!'
        }
        failure {
            // Actions to be performed if the build fails
            echo 'Build failed'
        }
    }
}
