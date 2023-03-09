pipeline {

          agent {
		  
		      label {
			  
			      label "built-in"
				  customWrokspace "/mnt/host-index"
			  }
		  }
		  
		  stages {
		  
		     stage ("on slave-1") {
			 
			     steps {
				 
				 sh "sudo rm -rf /var/www/html/*"
				 sh "sudo cp -r /mnt/host-index/index.html /var/www/html/"
				 sh "sudo chmod -R 777 /var/www/html/index.html"
				 
			
				 }
			 
			 
			 }
		  
		  
		  
		  
		  
		  }



}
