pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/home/pradip/project"
			
		}		
	}	

  stages {
    stage("facebook1") {
	    steps {
	       sh "sudo chmod -R 777 /home"
               sh "ansible-playbook index.yaml --check"
      }
    }
  }	  
}
