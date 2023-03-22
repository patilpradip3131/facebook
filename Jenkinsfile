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
               sh "sudo ansible-playbook index.yaml --check"
      }
    }
  }	  
}
