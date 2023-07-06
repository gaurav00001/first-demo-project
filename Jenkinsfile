pipeline {
    agent any

    stages {
    
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
                curl -T target/first-demo-project-0.0.1-SNAPSHOT.jar "http://192.168.1.15:8081/artifactory/java-web-app/artifacts"
            }
        }
    }
}
