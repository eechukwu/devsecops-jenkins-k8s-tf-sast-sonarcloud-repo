pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=xxxxxxxxxx -Dsonar.organization=xxxxxxxxxx -Dsonar.host.url=https://sonarcloud.io -Dsonar.login='
			}
        } 
  }
}
