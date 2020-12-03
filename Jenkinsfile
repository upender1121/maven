pipeline {
    agent any 
    stages {
        stage ("compile stage") {
            steps {
			withMaven (maven: 'maven-3.6.3'){
			  bat 'mvn clean compile'               
            }
          }
        }
        stage ("package stage") {
		steps {
		    withMaven (maven: 'maven-3.6.3'){
			  bat 'mvn package'      
            }
          }
        }
   	} 
}
