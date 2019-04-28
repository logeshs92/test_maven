pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        build 'test1-build'
      }
    }
    stage("deploy") {
Parallel  {
stage(“deploy1”) {
  input {
	  message “press ok to continue”
	  submitter “admin”
	  parameters {
			  string{name: ’username’, defaultValue: ‘’user, description: ‘Username of the user pressing ok’
    }
      steps {
        build 'test1-deploy'
	echo “User: ${username} said ok”
      }
}
stage(“deploy2”) {
	steps {
		build ‘test1-deploy’
}
}
    }
    stage("test") {
      steps {
        build 'test1-test'
      }
    }
  }
}

