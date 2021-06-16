pipeline {
    agent any
      tools{
        maven 'maven'}
    
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/chitbolujayanth/abc.git'
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
                bat "mvn clean install"
                
            }
        }
        
        
    }
}
