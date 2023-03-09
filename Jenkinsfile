pipeline {

          agent {
		  
		      label {
			  
			      label "built-in"
				  customWorkspace "/mnt/host-index"
			  }
		  }
		  
		  stages {
		  
		     stage ("on master") {
			 
			     steps {
				 sh "sudo yum install httpd -y"
				 sh "sudo systemctl start httpd"    
				 sh "sudo rm -rf /var/www/html/*"
				 sh "sudo cp -r /mnt/host-index/index.html /var/www/html/"
				 sh "sudo chmod -R 777 /var/www/html/index.html"
				 
			
				 }
			 
			 
			 }
		  
		  
		  
		  
		  
		  }



}
