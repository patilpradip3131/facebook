pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt"
			
		}		
	}	

  stages {
    stage("facebook1") {
	    steps {      
               sh "ansible-playbook index.yaml --check"
      }
    }
  }	  
}
