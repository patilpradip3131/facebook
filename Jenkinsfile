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
               sh "ansible-playbook index.yaml --check"
      }
    }
  }	  
}
