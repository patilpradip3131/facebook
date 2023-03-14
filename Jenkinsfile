pipeline {
  agent {
        label {
		
		    label "slave-1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
      steps {
	sh "sudo rm -rf /mnt/jenkins-slave/workspace/"
        sh "sudo docker run -itdp 8080:80 --name container-1 /mnt/jenkins-slave/index.html:/usr/local/apache2/htdocs/index.html httpd httpd1       
      }
    }
  }
}
