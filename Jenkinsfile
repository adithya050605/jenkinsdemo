pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/adithya050605/jenkinsdemo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo "This is a build step"'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "This is a test step"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'echo "This is a deploy step"'
            }
        }
    }
}
