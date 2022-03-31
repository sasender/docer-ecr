
pipeline {
  agent { label 'slave' } 
  
    stages {
	    stage ('git clone') {
	    
		    steps {
		     git 'https://github.com/sasender/docer-ecr.git'
		  
		    }
		}
		
		stage ('docker build') {
            
            steps {
                sh 'docker build -t sasender/spring-boot-mongo .'
                
            }
		}
		
	}
}
