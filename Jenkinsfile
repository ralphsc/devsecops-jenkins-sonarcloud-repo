pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecgurubuggywebapp -Dsonar.organization=asecgurubuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=662bc6244183c307a68106f067885d8e2e675b45'
			}
        } 
  }
}
