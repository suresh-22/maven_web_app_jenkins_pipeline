pipeline{
    agent any
    stages{
      		 stage('GetCode'){
            		steps{
		  		git branch: 'main', credentialsId: 'pipeline', url: 'https://github.com/suresh-22/maven_web_app_jenkins_pipeline.git'
            }
         }      
       		stage('Build'){
            		steps{
                		sh 'mvn clean compile'
            }
         }       
    }
}

