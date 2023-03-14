pipeline {
  agent {
        label {
		
		    label "slave-1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
      steps {
	sh "rm -rf /mnt/jenkins-slave/workspace/"
        sh "docker run -itdp 8080:80 --name container-1 /mnt/jenkins-slave/index.html:/usr/local/apache2/htdocs/index.html httpd httpd1       
      }
    }
  }
}
