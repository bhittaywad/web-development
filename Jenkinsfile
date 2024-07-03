pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
              sh  'building application'
            }
        }
        stage('Test') { 
            steps {
                sh 'testing application'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'deploying application'
            }
        }
    }
}
