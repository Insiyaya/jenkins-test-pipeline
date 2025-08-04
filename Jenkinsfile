// Jenkinsfile
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repo...'
                git url: 'https://github.com/insiyaya/jenkins-test-pipeline.git', branch: 'master'
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
