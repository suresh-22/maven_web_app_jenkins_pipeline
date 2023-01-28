pipeline{
    agent any
	 environment {
        	PATH = "$PATH:/opt/apache-maven-3.8.7/bin"
    }
    stages{
      		 stage('GetCode'){
            		steps{
		  		git branch: 'main', credentialsId: 'pipeline', url: 'https://github.com/suresh-22/maven_web_app_jenkins_pipeline.git'
            }
         }      
       		stage('Build'){
            		steps{
                		sh 'mvn clean install'
            }
         }       
    }
}

