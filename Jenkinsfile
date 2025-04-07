pipeline {
  agent any
  tools { 
        maven 'maven3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=suheab-buggy-web-app -Dsonar.organization=suheab-buggy-web-app -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c8d80dd5250bafaf826a4d56215216b151cca1af'
			}
    }

    }
}
