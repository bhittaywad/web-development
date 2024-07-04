pipeline {
    agent any
    environment{
        JAWAD_SERVER = credentials('prod-server')
    }
    stages {
        stage('build-dev') {
            when {
                expression {
                    BRANCH_NAME == 'ahmad'
                }
            }
            
            steps {
                echo "Hello World ${JAWAD_SERVER}"
            }
        }
        stage('push-dev') {
            when {
                expression {
                    BRANCH_NAME == 'ahmad'
                }
            }
            steps {
                echo "image has build successfully"
            }
        }

        stage('deploy-dev') {
            when {
                expression {
                    BRANCH_NAME == 'ahmad'
                }
            }
            steps {
                echo "imgae pushed"
            }
        }

        
        stage ('build-staging') {
            when {
                expression {
                    BRANCH_NAME == 'jenkins-job'
                }
            }
            steps {
                echo 'Build staging image'
            }
        }

        stage ('push-staging') {
            when {
                expression {
                    BRANCH_NAME == 'jenkins-job'
                }
            }
            steps {
                echo 'push staging image'
            }
        }

        stage ('deploy-staging') {
            when {
                expression {
                    BRANCH_NAME == 'jenkins-job'
                }
            }
            steps {
                echo 'deploy staging image'
            }
        }

        stage ('build-prod') {
            when {
                expression {
                    BRANCH_NAME == 'master'
                }
            }
            steps {
                echo 'Build prod image'
            }
        }

        stage ('push-prod') {
            when {
                expression {
                    BRANCH_NAME == 'master'
                }
            }
            steps {
                echo 'push prod image'
            }
        }
        stage ('deploy-prod') {
            when {
                expression {
                    BRANCH_NAME == 'master'
                }
            }
            steps {
                echo 'deploy prod image'
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

