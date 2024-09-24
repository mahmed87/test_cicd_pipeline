pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'ec643147-1277-4126-8006-e9bb241b8db4', branch: 'main', url: 'https://github.com/mahmed87/test_cicd_pipeline/tree/main'
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
