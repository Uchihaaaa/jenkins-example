pipeline {
    agent any 
    stages {
        stage('Build') { 
        	stages{
        		withMaven(maven : 'maven_3_5_3'){
            		sh 'mvn clean compile'
            	}
        	}
        }
        stage('Test') { 
            stages{
        		withMaven(maven : 'maven_3_5_3'){
            		sh 'mvn test'
            	}
        	}
        }
        stage('Deploy') { 
            stages{
        		withMaven(maven : 'maven_3_5_3'){
            		sh 'mvn deploy'
            	}
        	}
        }
    }
}
