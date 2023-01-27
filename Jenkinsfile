pipeline{
    agent any
    stages{
      		 stage('GetCode'){
            		steps{
		  		git branch: 'main', credentialsId: 'pipeline', url: 'https://github.com/suresh-22/maven_web_app_jenkins_pipeline.git'
            }
         }      
	    
	stages {
        	stage ('Initialize') {
            		steps {
                	sh '''
                    		echo "PATH = ${PATH}"
                    		echo "M2_HOME = ${M2_HOME}"
            		'''
		}
        }
       		stage('Build'){
            		steps{
                		sh 'mvn compile'
            }
         }       
    }
}
