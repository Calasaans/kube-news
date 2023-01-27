pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("jorgecalasans/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}