pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp3410 -Dsonar.organization=asgbuggywebapp3410 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=edf2b50c531961bc526d3ee65d8c9e735fa89371'
			}
        } 
  }
}
