pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt/project"
			
		}		
	}	

  stages {
    stage("Deploy facebook-1") {
      steps {
       sh "sudo chmod -R 777 /mnt"      
       sh "ansible-playbook index.yaml --check"
      }
    }
  }	  
}
