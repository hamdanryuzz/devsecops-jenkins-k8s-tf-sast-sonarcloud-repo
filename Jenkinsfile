pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityryuz -Dsonar.organization=asecurityryuz -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=cef349fa1c1bcfbbf4118e011b798b2187cff0a6'
			}
        } 
  }
}
