pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sampleapp-devsecops_sampleproject -Dsonar.organization=sampleapp-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e80fbad06e6e837fb08d2e9fda2bae5081fe580cn'
			}
        } 
  }
}
