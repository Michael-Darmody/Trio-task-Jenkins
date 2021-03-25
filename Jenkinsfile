pipeline {
    agent any
    enviorment {

    }
    stages {
        stage("Build") {
            steps {
                sh "docker-compose build --parallel"
            }
        }
        stage("Push") {
            steps {
                sh "docker-compose push"
            }
        }
        stage("Deploy") {
            steps {
                sh "docker-compose up -d"
            }
        }
    }
}