pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES2UG22CS640-1 hello.cpp'   // Compiles hello.cpp
                    echo 'Build Stage Successful'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './hello_exec'  // Runs the compiled executable
                    echo 'Test Stage Successful'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application... (placeholder)'
                echo 'Deployment Successful'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
