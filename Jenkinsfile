pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS059-1 ankitha.cpp'
                echo 'build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG20CS059-2'
                echo 'test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'pipeline failed'
                }
            
        
    }
}
