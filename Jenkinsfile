pipeline {
    agent any 
    stages {
        stage('Hello World') {
            steps {
                sh '''
                docker --version
                python --version
                docker build -t my_flask_image_1 .
                docker run -it -p 5000:5000 my_flask_image_1
                ls -ltr

                '''
            }
        }
    }
}