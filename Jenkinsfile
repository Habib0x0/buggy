pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggy -Dsonar.organization=buggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3f612c8d827a90a6c93df8d69ca1bddac807f1b4'
			}
        } 
  }
}