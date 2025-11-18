pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World from Jenkins!'
            }
        }
    }
}

pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Jenkins gjør checkout automatisk
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
                // Eksempel på test-kommando
                // Hvis du har Python unittests:
                // sh 'python -m unittest discover -s tests'

                echo 'Running tests...'
                // Simulere test pass
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


