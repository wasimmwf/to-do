pipeline {
    agent any 
    stages {
        stage('Hello World') {
            steps {
                sh '''
                docker --version
                python --version
                docker build -t my_flask_image_1 .
                '''
            }
        }
    }
}