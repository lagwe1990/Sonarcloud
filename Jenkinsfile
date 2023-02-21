pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguruwebapp -Dsonar.organization=asecurityguruwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=93c8dd98cae099cf06b39a9536667c336cecbb86'
			}
        } 
  }
}
