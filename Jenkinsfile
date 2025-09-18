pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code from branch: ${env.BRANCH_NAME}"
                
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // e.g. sh './deploy.sh'
            }
        }
    }
}
