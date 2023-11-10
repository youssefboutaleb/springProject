pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the GitHub repository
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Build the project (Maven example)
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run tests (if applicable)
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application (if applicable)
                // Add deployment steps here
            }
        }
    }

    post {
        success {
            // Actions to be taken if the build is successful
            echo 'Build successful! Deploying...'
            // Add additional post-build actions here
        }
        failure {
            // Actions to be taken if the build fails
            echo 'Build failed! Notify the team...'
            // Add additional post-failure actions here
        }
    }
}
