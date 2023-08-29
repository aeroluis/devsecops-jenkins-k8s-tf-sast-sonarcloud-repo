pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=luismi -Dsonar.organization=luismi -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=092df89bf68dab34a4e204fd0c176a078e7dcfe2'
			}
        } 
  }
}
