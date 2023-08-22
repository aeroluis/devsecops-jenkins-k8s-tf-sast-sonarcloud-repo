pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=organization-luismi_organization-luismi -Dsonar.organization=organization-luismi -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f44c8f82a3a52bd33d83d96fa041834c3a8a634d'
			}
        } 
  }
}
