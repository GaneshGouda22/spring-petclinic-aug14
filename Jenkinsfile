pipeline {
    agent any
    tools {
        maven 'MAVEN_3.9.8'
    }
    stages {
        stage('GIT') {
            steps { 
               git url: 'https://github.com/spring-projects/spring-petclinic.git',
                   branch: 'main'
            }
        }
        stage('build'){
            steps {
                sh 'mvn clean package'
            }
        }
    
        
    }
}