pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code from branch: ${env.BRANCH_NAME}"
                // Jenkins automatically checks out the branch for multibranch pipelines
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'mvn clean package'  // example for Java/Maven project
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'  // example for Java/Maven project
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
