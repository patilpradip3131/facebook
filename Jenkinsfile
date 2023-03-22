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
       sh "ansible-playbook test.yaml --check"
      }
    }
  }	  
}
