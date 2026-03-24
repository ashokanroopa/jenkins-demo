pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo "Building the application..."
            }
        }

        stage('Parallel Stage') {
            parallel {

                stage('Test') {
                    steps {
                        echo "Running tests..."
                    }
                }

                stage('Code Check') {
                    steps {
                        echo "Checking code..."
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}
