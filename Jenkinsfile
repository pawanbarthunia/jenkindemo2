pipeline {
    agent any 
    stages {
	
        stage('Compile Stage') { 
            steps{
				withMaven(maven:'Maven_home'){
				 sh 'mvn clean compile'
			  }
			 }
			}
		stage('Testing Stage') { 
            steps{
				withMaven(maven:'Maven_home'){
				 sh 'mvn test'
			  }
			 }
			}
		stage('Deploy Stage') { 
            steps{
				withMaven(maven:'Maven_home'){
				 sh 'mvn deploy'
			  }
			 }
			}			
			
}
