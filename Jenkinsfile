pipeline {
    agent any

    stages {
        stage('test-dev') {
            when {
                expression {
                    BRANCH_NAME == 'ahmad'
                }
            }
            
            steps {
                echo 'Hello World'
            }
        }
        stage('build-dev') {
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

        stage('push-dev') {
            when {
                expression {
                    BRANCH_NAME== 'ahmad'
                }
            }
            steps {
                echo "pushing the iamge"
            }
        }


        stage ('test-staging'){
            steps {
                echo "testing the iamge"
            }
        }   
        }
        stage ('build-staging') {
        
            steps {
                echo 'Build staging image'
            }
        }

        stage ('push-staging') {
            
            steps {
                echo 'push staging image'
            }
        }

        stage ('deploy-staging') {
            
            steps {
                echo 'deploy staging image'
            }
        }

      
        stage ('test-prod'){
          when {
                expression {
                    BRANCH_NAME== 'master'
                }
            }
            steps {
                echo "testing the iamge"
            }
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
} 

