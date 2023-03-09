pipeline {

          agent {
		  
		      label {
			  
			      label "built-in"
				  customWrokspace "/mnt/host-index"
			  }
		  }
		  
		  stages {
		  
		     stage ("p") {
			 
			     steps {
				 
				 sh "sudo rm -rf /root/.m2/repository"
				 sh "sudo mvn clean install"
				 sh "sudo cp -r /mnt/project/game-of-life/gameoflife-web/target/gameoflife.war /mnt/server/apache-tomcat-9.0.73/webapps"
				 
			
				 }
			 
			 
			 }
		  
		  
		  
		  
		  
		  }



}
