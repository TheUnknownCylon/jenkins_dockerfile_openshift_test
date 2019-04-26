pipeline {
    agent none
    stages {
        stage('Stage 1') {
            agent { dockerfile true }
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'echo $REMCO'
            }
        }
        stage('Stage 2') {
            agent { dockerfile true }
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'echo $REMCO'
            }
        }
        stage('Stage 3') {
            agent {
                docker 'openjdk:8-jre' 
                options { skipDefaultCheckout() }
            }
            steps {
                sh 'ls'
                sh 'java -version'
            }
        }
    }
}
