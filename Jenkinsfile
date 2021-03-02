pipeline {
	agent any
	tools {
    	maven 'my_mvn'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/mansgupt11/CMtools_Project1-.git'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
        stage('install') {
        	steps {
        	sh "mvn clean install"  	 
        	}
    	}	 
   }
