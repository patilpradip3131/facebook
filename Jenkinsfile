pipeline {
  agent {
        label {
		
		    label "slave-1"
		}
  }
  stages {
    stage('Deploy to Container-2') {
	    steps {
               sh "sudo docker run -itdp 8080:80 --name container-1 httpd"
	       sh "sudo docker cp /mnt/jenkins-slave/workspace/docker-multi_master/index.html container-2:/usr/local/apache2/htdocs"    
      }
    }
  }
}
