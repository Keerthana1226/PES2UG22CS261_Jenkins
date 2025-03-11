pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Compile the C++ code
                sh 'g++ -o PES2UG22CS261-1 main.cpp'
                echo 'Build stage completed'
            }
        }
        stage('Test') {
            steps {
                // Run the compiled executable
                sh './PES2UG22CS261-1'
                echo 'Test stage completed'
            }
        }
        stage('Deploy') {
            steps {
                // Placeholder for deployment steps
                echo 'Deployment completed'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
        success {
            echo 'Pipeline completed successfully'
        }
    }
}
