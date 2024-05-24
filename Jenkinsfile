pipeline {
    agent none
    stages {
        ...
            stage("Build Docker Image") {
            agent any
            environment {
        HOME = "${env.WORKSPACE}"
        }
            steps {
               script {
                dockerImage = docker.build("<docker image name>:${env.BUILD_ID}")
               }
            }
        }
        ...
    }
}