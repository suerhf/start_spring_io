pipeline {
	agent any
	tools {
    	maven 'my_maven'
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

