pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ hello_337.cpp -o hello_337'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './hello_337'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployement Successfull"
            }
        }
    }
    
    post {
        failure {
            echo "Pipeline failed"
        }
    }
}
