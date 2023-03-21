pipeline {
  agent {
     label {
	     label "built-in"
		 customWorkspace "/mnt"
	 
	 }
  }
  stages {
    stage("deploy facebook-1") {
	    steps {
	        sh "ansible-playbook index.yaml --check"
	      
      }
    }
  }
}
