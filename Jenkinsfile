pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'mvn clean package' // Adjust for your build tool
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test' // Replace with appropriate test commands
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                sh 'oc rollout latest dc/myapp' // Adjust deployment config
            }
        }
    }
}
