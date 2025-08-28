pipeline {
    agent any

    tools {
        maven 'Maven-3.9'    
        jdk 'JDK17'        
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/jenkins-docs/simple-java-maven-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
