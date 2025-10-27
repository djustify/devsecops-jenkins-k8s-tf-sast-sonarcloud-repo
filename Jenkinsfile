pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=justifywebapp -Dsonar.organization=justifywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4dcbf713f1bfcb4b2075ff354ce8f51ac086bb10'
			}
        } 
  }
}
