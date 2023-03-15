pipeline {
  agent {
        label {
		
		    label "slave-1"
			customWorkspace "/mnt/vol2"
		}
  }
  stages {
    stage('Deploy to Container-2') {
	    steps {
	       sh "sudo docker stop container-2"
               sh "sudo docker rm container-2"
	       sh "sudo docker volume create my-volume-2"
	       sh "sudo cp /mnt/vol2/index.html /var/lib/docker/volumes/my-volume-2/_data"
	       sh "sudo docker run -itdp 8080:80 -v my-volume-2:/usr/local/apache2/htdocs --name container-2 httpd"
	      
      }
    }
  }
}
