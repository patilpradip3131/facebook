pipeline {
  agent {
        label {
		
		    label "slave-1"
			customWorkspace "/mnt/vol1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
	    steps {
	       sh "sudo docker stop container-1"
               sh "sudo docker rm container-1"
	       sh "sudo docker run -itdp 80:80 -v /mnt/vol1/index.hmtl:/usr/local/apache2/htdocs --name container-1 httpd"
	       sh "docker exec container-1 chmod 777 /usr/local/apache2/htdocs/index.html"    
      }
    }
  }
}
