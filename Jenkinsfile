pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dinosecgurubuggywebapp -Dsonar.organization=dinosecgurubuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=22c54e301947d90d876ef04de6bb1cfe6cc65387'
			}
        } 
  }
}
