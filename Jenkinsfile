pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopstest-001/devsecopstest-001 -Dsonar.organization=devsecopstest-001 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=767a0da52df3c04a6f31db26e115a44b5eb1893d'
			}
        } 
  }
}
