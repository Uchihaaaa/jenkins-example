pipeline {
    agent any
	
	tools{
		maven 'maven_3_5_2'
		jdk 'java8'
	}
	
    stages {
        stage ('Compile Stage') {

            steps {
                echo "Compile"
            }
        }

        stage ('Testing Stage') {

            steps {
                echo "Testing"
            }
        }


        stage ('Deployment Stage') {
            steps {
               echo "Deployment"
            }
        }
    }
}