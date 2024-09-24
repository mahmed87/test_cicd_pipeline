pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-pat-id', branch: 'main', url: 'https://github.com/mahmed87/test-cicd-pipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo Build step running'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo Tests are passing'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                sh 'echo Deployment step executed'
            }
        }
    }
}
