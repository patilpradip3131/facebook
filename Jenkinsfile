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
        ansiblePlaybook credentialsId: 'ansible-creds',
          inventory: 'hosts/host1.ini',
          playbook: '/mnt/project/index.yaml'
      }
    }
  }	  
}
