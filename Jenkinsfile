pipeline {
    
    agent any
    tools {
        maven 'Maven 3.6.9'
        jdk 'jdk11'
    }
    stages {
        stage('Fetch code') {
            steps {
                echo 'Build'
                git branch: 'master', url: 'https://github.com/sivajiseru/java.git'
            }
        }
        
       
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
           
        }
    }
        stage('Build') {
            steps {
                echo 'Build'
                sh 'mvn install'
            }
        }
        stage('Test') {
            steps {
                echo 'Test'
                //sh 'mvn test'
            }
        }
    
}
