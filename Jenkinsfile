pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out the repository...'
                git branch: 'main', url: 'https://github.com/adithya050605/jenkinsdemo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo "This is the build step"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "This is the test step"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                sh 'echo "This is the deploy step"'
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
