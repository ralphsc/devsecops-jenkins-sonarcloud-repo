pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecgurubuggywebapp -Dsonar.organization=asecgurubuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=Your-Code-Here'
			}
        } 
  }
}
