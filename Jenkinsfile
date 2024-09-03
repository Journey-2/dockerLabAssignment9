pipeline {
    agent any
    stages {
        stage('Build Image') {
            steps {
                bat 'docker build -t "assignment9-image:1.0" .'
            }
        }
        stage('Run Container') {
            steps {
                bat 'docker run -d --name assignment9-container assignment9-image:1.0'
            }
        }
    }
}
