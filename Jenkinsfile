pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t hello-java .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm hello-java'
            }
        }
    }
}
