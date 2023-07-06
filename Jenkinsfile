pipeline {
    agent any

    stages {

        stage('Maven') {
            steps {
                sh 'M2_HOME='/opt/apache-maven-3.9.3''
                sh 'PATH="$M2_HOME/bin:$PATH"'
                sh 'export PATH'
            }
        }        
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
