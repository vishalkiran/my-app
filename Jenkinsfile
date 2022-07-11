pipeline {
    agent any
    
    tools {
    maven 'maven8'
    }

    stages {
        stage('git-clone') {
            steps {
                git 'https://github.com/vishalkiran/my-app'
            }
        }
        stage('maven-build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
