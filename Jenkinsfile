pipeline {
    agent any
    tools {
        maven 'maven'  // The name you provided during Maven configuration
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main' , url: 'https://github.com/mohamedahmed22796/Hello-World-with-Java.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
