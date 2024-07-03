pipeline {
    agent any
    
    stages {
        stage('Hello') {
            steps {
                // Define the steps to be executed in this stage
                echo 'Hello world'
            }
        }
        // You can define more stages here as needed
    }
    
    // Optionally, define post actions, such as notifications or cleanup steps
    post {
        always {
            // Actions to be performed after all stages are executed
            echo 'Pipeline finished'
        }
    }
}
