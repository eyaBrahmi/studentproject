pipeline {
    agent any

    tools {
        jdk 'jdk21'
    }

    stages {

        stage('Check Java') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
