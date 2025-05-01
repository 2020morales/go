pipeline {
    agent { label 'agent3' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/2020morales/go.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}
