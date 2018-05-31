pipeline {
    agent any
    tools {
        maven 'mavenJenkins' 
    }
    stages {
        stage ('Compile Stage') {
            steps {
                sh "mvn clean compile"
            }
        }
        stage ('Testing Stage') {
            steps {
              	sh 'mvn test'
            }
        }
    }
}