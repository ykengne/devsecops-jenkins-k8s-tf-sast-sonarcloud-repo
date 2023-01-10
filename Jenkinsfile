pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=yanndevsecops -Dsonar.organization=yanndevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e39e8af8fe2ed8f765a2658fe00b6cee345a0655'
			}
        } 
  }
}
