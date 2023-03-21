pipeline {
	agent {
		label {
		   
			label "built-in"
			customWorkspace "/mnt/project"
			
		}		
	}	

  stages {
    stage('Deploy q1 branch') {
      steps {
        ansiblePlaybook credentialsId: 'id_rsa',
          inventory: '/etc/ansible/hosts',
          playbook: '/mnt/project/index.yaml'
      }
    }
  }	  
}
