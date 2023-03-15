pipeline {
  agent {
        label {
		
		    label "slave-1"
			CustomWorkspace "/mnt/vol1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
	    steps {
	       sh "sudo docker stop container-1"
               sh "sudo docker rm container-1"
	       sh "sudo docker run -itdp 80:80 -v vol1:/usr/local/apache2/htdocs --name container-1 httpd"
      }
    }
  }
}
