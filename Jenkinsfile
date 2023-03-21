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
	        sh "command: cd /mnt/project/ | ansible-playbook index.yaml"
             
	      
      }
    }
  }
}
