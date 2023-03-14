pipeline {
  agent {
        label {
		
		    label "slave-1"
		}
  }
  stages {
    stage('Deploy to Container-1') {
      steps {
        sh "docker run -itdp 8080:80 --name container-1 /mnt/jenkins-slave/index.html:/usr/local/apache2/htdocs/index.html httpd httpd1"
      }
    }
    stage('Deploy to Container-2') {
      steps {
        
        sh "docker run -itdp 8081:80 --name container-2 /mnt/jenkins-slave/index.html:/usr/local/apache2/htdocs/index.html httpd httpd2"
        
      }
    }
    stage('Deploy to Container-3') {
      steps {
        
        sh "docker run -itdp 8082:80 --name container-3 /mnt/jenkins-slave/index.html:/usr/local/apache2/htdocs/index.html httpd httpd3"
        
      }
    }
  }
}
