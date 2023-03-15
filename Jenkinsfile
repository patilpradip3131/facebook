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
	       sh "sudo docker run -itdp 80:80 -v /var/lib/docker/volumes/vol1/_data/index.html:/usr/local/apache2/htdocs --name container-1 httpd"
      }
    }
  }
}
