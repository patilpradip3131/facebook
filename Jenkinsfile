pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt/project/"
			
		}		
	}	

  stages {
    stage("Deploy facebook-1") {
	    steps {      
               sh "sudo ansible-playbook index.yaml --check"
      }
    }
  }	  
}
