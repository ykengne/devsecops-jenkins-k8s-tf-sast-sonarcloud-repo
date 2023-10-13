pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=yandevsecop -Dsonar.organization=yandevsecop -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9e374df2670c9396917f10c0418172a68c201b71'
			}
        } 
  }
}
