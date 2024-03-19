pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/DEL-ORG/s6rasheedat-practices.git'
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
