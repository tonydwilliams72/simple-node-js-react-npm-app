pipeline {
    agent { docker { image 'node:8.12.0' } }
    environment {
        HOME = '.'
    }
    stages {
        stage('Clone') {
            steps {
                git branch: 'master',
                    credentialsId: '121231k3jkj2kjkjk',
                    url: 'https://myserver.com/my-repo.git'
            }
        }
        stage('Build') {
            steps {
                sh "npm install"
            }
        }
    }
}