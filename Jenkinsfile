pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=finalprojectbuggywebapp -Dsonar.organization=finalprojectbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f502da81e99f9df816ea4f78c9026879661db736'
			}
        } 
  }
}
