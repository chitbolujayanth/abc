pipeline {
    agent any
      tools{
        maven 'maven'}
    
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/chitbolujayanth/abc.git'
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
                sh "mvn clean install"
                
            }
        }
        
        
    }
}
