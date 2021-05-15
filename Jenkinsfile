pipeline {
	agent any
	tools {
    	maven 'my_maven'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git branch: 'main', url: 'git@github.com:suerhf/start_spring_io.git'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "cd calculator && mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "cd calculator && mvn test"       	 
       	}
        stage("Package") {
     		steps {
		sh "cd caluculatr && mvn package"
}
}
}

