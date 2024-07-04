pipeline {
    agent any

    stages {
        stage('Hello') {
            when {
                expression {
                    BRANCH_NAME == "ahmad"
                }
            }
            steps {
                echo 'Hello World'
            }
        }
        stage('build-image') {
            steps {
                echo "image has build successfully"
            }
        }

        stage('push-image') {
            steps {
                echo "imgae pushed"
            }
        }
    }
  post {
      success {
          echo 'Pipeline seccess'
      }
      failure{
          echo 'pipeline failed'
      }
  }  
} 
}
