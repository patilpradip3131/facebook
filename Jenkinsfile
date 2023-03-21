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
		sh "sudo chmod -R 644 /mnt/project   
	        sh "ansible-playbook index.yaml --check"
	      
      }
    }
  }
}
