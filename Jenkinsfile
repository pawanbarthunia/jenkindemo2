pipeline {
    agent any 
    stages {
	
        stage('Compile Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool 3.6.3}/bin"] ){
				 sh 'mvn clean compile'
			  }
			 }
			}
		stage('Testing Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool 3.6.3}/bin"] ){
				 sh 'mvn test'
			  }
			 }
			}
		stage('Deploy Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool 3.6.3}/bin"] ){
				 sh 'mvn deploy'
			  }
			 }
			}			
			
 }
}