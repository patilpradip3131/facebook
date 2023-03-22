pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/root/project"
			
		}		
	}	

  stages {
    stage("facebook1") {
	    steps {      
               sh "ansible-playbook -i /mnt/project index.yaml --check"
      }
    }
  }	  
}
