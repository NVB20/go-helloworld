pipeline {
    agent any
    tools { go '1.4' }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'go version'
                sh 'go run main.go'
                sh 'go build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'go test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}