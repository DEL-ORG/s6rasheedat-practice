options {
    skipDefaultCheckout()
}

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/DEL-ORG/s6rasheedat-practices.git'
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
