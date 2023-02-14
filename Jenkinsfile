pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG20CS012.cpp'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh './a.out'
                echo 'Test Successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }  
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
