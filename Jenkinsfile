pipeline { 
    agent any 
    tools {
        go 'go-1.14'
    }
    environment {
        GO111MODULE='on'
    }
    stages {
        stage('Test') { 
            steps { 
                git 'https://github.com/kodekloudhub/go-webapp-sample.git'
                sh 'go test ./...'
            }
        }
    }
}
