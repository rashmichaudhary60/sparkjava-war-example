pipeline {
    agent any

    environment {
         PATH = "/opt/maven/bin:$PATH"
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/rashmichaudhary60/sparkjava-war-example.git' , branch: 'master'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}


