pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
              sh 'docker build --no-cache -t babusai/project-two .'
            }
        }

        stage('Push to Docker Hub') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'dockerhub', usernameVariable: 'USER', passwordVariable: 'PASS')]) {
                    sh 'echo $PASS | docker login -u $USER --password-stdin'
                    sh 'docker push babusai/project-two'
                }
            }
        }
    }
}
