pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'clean install'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
