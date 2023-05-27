pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritygroupkey -Dsonar.organization=asecuritygroupkey -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7a8755db3115d05c0c082731c262b45f6f7c5e89'
			}
        } 
  }
}
