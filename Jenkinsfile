pipeline {
    agent any
    tools {
        maven 'M3'
        jdk 'JDK17'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'mvn test'
            }
        }
        stage('Deliver') {
            when { branch 'main' }
            steps {
                echo 'Deploying to Production...'
                sh 'mvn package'
            }
        }
    }
    post {
        always {
            junit 'target/surefire-reports/*.xml'
        }
    }
}