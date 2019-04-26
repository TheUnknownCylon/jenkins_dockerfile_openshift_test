pipeline {
    agent { dockerfile true }
    stages {
        stage('Stage 1') {
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'echo $REMCO'
            }
        }
        stage('Stage 2') {
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'echo $REMCO'
            }
        }
        stage('Stage 3') {
            agent { docker 'openjdk:8-jre' }
            steps {
                sh 'ls'
                sh 'java -version'
            }
        }
    }
}
