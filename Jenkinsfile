pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        build 'test1-build'
      }
    }
    stage("deploy") {
	     input{
		message "Press Ok to continue"
		submitter "admin"
		parameters {
			string(name:'username', defaultValue: 'user', description: 'Username of the user pressing Ok')
		}
	}
	parallel  {
	stage(“deploy1”) {
 	
      steps {
        build 'test1-deploy'
	echo "User: ${username} said Ok."
      }
}
stage(“deploy2”) {
	steps {
		echo "deploy2" 
		echo "User: ${username} said Ok."
}
}
    }
    }
    stage("test") {
      steps {
        build 'test1-test'
      }
    }
  }
  post {
  success {
        echo "project deployed and tested successfully"
      }
    }
}
