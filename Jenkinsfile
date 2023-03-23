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
	       sh "pwd"
	       sh "ls-ltra"
               sh "sudo su -c ansible-playbook index.yaml"
      }
    }
  }	  
}
