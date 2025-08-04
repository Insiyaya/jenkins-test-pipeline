// Jenkinsfile
pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repo...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Running build...'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}
