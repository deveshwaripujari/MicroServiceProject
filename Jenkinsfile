pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK11'
    }
    environment {
        GITHUB_CREDENTIALS = credentials('1') // Replace with your actual credentials ID
    }
    stages {
        stage('Checkout') {
            steps {
                git credentialsId: GITHUB_CREDENTIALS, url: 'https://github.com/deveshwaripujari/MicroPro.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Docker Build') {
            steps {
                script {
                    docker.build('spring-boot-microservice')
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    docker.image('spring-boot-microservice').run('-p 8081:8080')
                }
            }
        }
    }
}
