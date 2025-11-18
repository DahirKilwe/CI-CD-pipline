pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checked out source code'
            }
        }

        stage('Build') {
            steps {
                echo 'Build step - can compile code here'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Her simulerer vi at alle tester passer
                sh 'echo "All tests passed!"'
            }
        }

        stage('Finish') {
            steps {
                echo 'Pipeline finished successfully!'
            }
        }
    }
}
