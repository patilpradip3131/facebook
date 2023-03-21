pipeline {
  agent {
     label {
	     label "built-in"
		 customWorkspace "/mnt/project"
	 
	 }
  }
  stages {
    stage("deploy facebook-1") {
	    steps {
		  
	        ansiblePlaybook(
                    playbook: '/mnt/project/index.yml',
                    inventory: '/etc/ansible/hosts',
                    extras: '-e "variable=value"'
             )
	      
      }
    }
  }
}
