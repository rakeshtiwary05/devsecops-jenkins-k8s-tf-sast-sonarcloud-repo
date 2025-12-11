pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=tiwaryra_buggy_app -Dsonar.organization=tiwaryra_buggy_app -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4c8992d47e32bad367062924eb5829723fb7cf03'
			}
        } 
  }
}
