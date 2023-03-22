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
        ansiblePlaybook credentialsId: 'id_rsa',
          inventory: 'hosts',
          playbook: '/mnt/project/index.yaml'
      }
    }
  }	  
}
