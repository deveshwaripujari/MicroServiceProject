pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'JDK11'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/spring-boot-microservice.git'
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
                    docker.image('spring-boot-microservice').run('-p 8080:8080')
                }
            }
        }
    }
}
