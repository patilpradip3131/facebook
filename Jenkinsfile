pipeline {
  agent {
        label {
		
		    label "slave-1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
	    steps {
               sh "sudo docker run -itdp 8080:80 -v /mnt/jenkins-slave/workspace/docker-multi_master/index.html:/usr/local/apache2/htdocs httpd"      
      }
    }
  }
}
