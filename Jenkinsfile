pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt/project"
			
		}		
	}	

  stages {
    stage("facebook1") {
	    steps {
	       sh "sudo chmod -R 777 /mnt"
               sh "ansible-playbook -u index.yaml --check"
      }
    }
  }	  
}
