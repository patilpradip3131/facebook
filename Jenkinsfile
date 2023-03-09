pipeline {

          agent {
		  
		      label {
			  
			      label "slave-1"
				  customWorkspace "/mnt/host-index"
			  }
		  }
		  
		  stages {
		  
		     stage ("host on slave-1") {
			 
			     steps {
				 sh "sudo rm -rf /var/www/html/*"
				 sh "sudo cp -r /mnt/host-index/index.html /var/www/html/"
				 sh "sudo chmod -R 777 /var/www/html/index.html"
				
				 }
			 
			 
			 }
		  
		  
		  
		  
		  
		  }



}
