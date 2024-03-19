pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                script {
                    checkout([$class: 'GitSCM', branches: [[name: 'main']], 
                        userRemoteConfigs: [[url: 'https://github.com/DEL-ORG/s6rasheedat-practices.git']]])
                }
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
    }
}
