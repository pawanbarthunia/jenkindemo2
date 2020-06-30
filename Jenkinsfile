pipeline {
    agent any 
    stages {
	
        stage('Compile Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ){
				 sh 'mvn clean compile'
			  }
			 }
			}
		stage('Testing Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ){
				 sh 'mvn test'
			  }
			 }
			}
		stage('Deploy Stage') { 
            steps{
				withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ){
				 sh 'mvn deploy'
			  }
			 }
			}			
			
 }
}