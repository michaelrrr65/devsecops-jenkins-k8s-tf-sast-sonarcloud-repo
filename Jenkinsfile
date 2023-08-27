pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebby -Dsonar.organization=asgbuggywebby -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2dcd38f3a774582274e9d3214e94a4b37ca6cdc9'
			}
        } 
  }
}
