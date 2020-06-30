pipeline {
    agent any 
    stages {
	
        stage('Compile Stage') { 
            steps{
				withEnv(maven:'Maven_home'){
				 sh 'mvn clean compile'
			  }
			 }
			}
		stage('Testing Stage') { 
            steps{
				withEnv(maven:'Maven_home'){
				 sh 'mvn test'
			  }
			 }
			}
		stage('Deploy Stage') { 
            steps{
				withEnv(maven:'Maven_home'){
				 sh 'mvn deploy'
			  }
			 }
			}			
			
 }
}