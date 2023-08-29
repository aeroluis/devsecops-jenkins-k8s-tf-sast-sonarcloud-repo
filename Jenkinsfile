pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=organization-luismi -Dsonar.organization=luismi -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e70b140f1b8a0b0780eb3304e697ec4cd75d29f2'
			}
        } 
  }
}
