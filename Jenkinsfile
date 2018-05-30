pipeline {
    agent any
    stages {
        stage ('Compile Stage') {
            steps {
                withMaven(maven : 'mavenJenkins') {
                    bat "mvn clean compile"
                }
            }
        }
        stage ('Testing Stage') {
            steps {
                withMaven(maven : 'mavenJenkins') {
                    bat 'mvn test'
                }
            }
        }
        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'mavenJenkins') {
                    bat 'mvn deploy'
                }
            }
        }
    }
}