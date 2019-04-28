pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        build 'test1-build'
      }
    }
    stage("deploy") {
    parallel  {
      stage(“deploy1”) {
        steps {
          build 'test1-deploy'
      }
    }
    stage(“deploy2”) {
	    steps {
		    echo "Sucess"
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
}

