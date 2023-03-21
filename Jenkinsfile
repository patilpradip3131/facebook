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
		sh "sudo chmod -R 777 /mnt"
	        ansiblePlaybook(
                 playbook: "ansible-playbook index.yaml --check"
             )
	      
      }
    }
  }
}
