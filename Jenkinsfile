pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checked out source code from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Legg inn kommandoen din for å bygge prosjektet
                // Eksempel for .NET: bat 'dotnet build MyProject.sln'
                // Eksempel for Java: bat 'javac src\\Main.java'
                bat 'echo Build completed successfully!'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Legg inn kommandoen for å kjøre tester
                // Eksempel for Python: bat 'python -m unittest discover -s tests'
                // Eksempel for Java: bat 'java -cp bin org.junit.runner.JUnitCore TestClass'
                bat 'echo All tests passed!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Legg inn deploy-kommandoen din
                // Eksempel: bat 'copy /Y build\\* C:\\inetpub\\wwwroot\\MyApp\\'
                bat 'echo Deployment completed!'
            }
        }

        stage('Finish') {
            steps {
                echo 'Pipeline finished successfully!'
            }
        }
    }
}
