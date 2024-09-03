pipeline {
    agent any

    stages {
        stage('Build Image') {
            steps {
                script {
                    def image = docker.build("assignment9-image:1.0")
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run -d --name assignment9-Containerassignment9-image:1.0'
                }
            }
        }
    }
}
