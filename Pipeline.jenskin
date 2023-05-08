pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/dervieni/DevOpsDemo']]])
            } 
        }
        stage('Test') { 
            steps {
                sh 'echo test'
            }
        }
        stage('Deploy') {
            steps {
               sh 'echo deploy'
            } 
        }
    }
}
