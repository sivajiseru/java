pipeline {
    
    agent any
   
    stages {
        stage('Fetch code') {
            steps {
                echo 'Build'
                git branch: 'master', url: 'https://github.com/sivajiseru/java.git'
                withMaven {
              sh "mvn clean verify"
            } 
            }
        }
    }
    
}
