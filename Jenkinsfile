pipeline {
    agent { 
        node {
            label 'docker' 
        }
    }

    stages {
        stage('Back-end') {
            
			steps {
			  sh 'whoami'
			}
			            
         
			steps {
			  sh 'mvn --version'
			}
        }
        stage('Front-end') {
		     
              agent {
			    docker { image 'node:7-alpine' }
			}
             steps {
			  sh 'node --version'
			}
            
		}
    }
}
