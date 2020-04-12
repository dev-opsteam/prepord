pipeline {
	agent any
	stages {
	stage ('SCm checkout') {
		steps {
			script {		
 	
           url 'https://github.com/dev-opsteam/prepord.git'
		}
	}
	}

    stages {
	stage ('build') {
		steps {
			script {		
 	
             sh 'mvn clean package'
		}
	}
	}
		
	stages {
	stage ('Junit test') {
		steps {
			script {		
 	
            junit '/target/test-reports/*.xml'
		}
	}
	}
 
    
		
	    }

	}

