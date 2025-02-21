pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'python -version'  // Modify for your project
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'hello.py/'  // Update as per your test command
            }
        }
    }
}
