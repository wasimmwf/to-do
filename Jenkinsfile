pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build . -t todo-app'
            }
        }
        stage('Run') {
            steps {
                sh 'docker run -d -p 5000:5000 todo-app'
            }
        }
    }
}