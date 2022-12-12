pipeline {
    agent any
    stages {
        stage('Fetch code') {
            steps {
                echo 'Build'
                //git branch: 'master', url: 'https://github.com/sivajiseru/java.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Build'
                //sh 'mvn install'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
                //sh 'mvn test'
            }
        }
    }
}
