pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=eecdevopsprojects -Dsonar.organization=eecdevopsprojects -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=19f14ac0ed842eebbd11c2206ecbfd69092b696e'
			}
        } 
  }
}
