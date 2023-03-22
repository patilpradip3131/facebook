pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt/project"
			
		}		
	}	

  stages {
    stage('Deploy facebook-1') {
      steps {
       sh "ansible-playbook /mnt/project/index.yaml -i /etc/ansible/hosts"
      }
    }
  }	  
}
