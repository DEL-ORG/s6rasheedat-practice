pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/your-repository.git'
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
