pipeline {
    agent { label 'uk-jenkins-test' }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Cirarshi/TravelMemory.git'
            }
        }
        stage('Install') {
            steps {
                sh 'cd backend; npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'cd backend; npm run build'
            }
        }
    }

}

