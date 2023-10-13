pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=yanndevsecopswebapp -Dsonar.organization=YannDevSecOpsWebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=979ec218c158fbf50f8f8276817b98e1e8aac0fb'
			}
        } 
  }
}
