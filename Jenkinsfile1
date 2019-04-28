pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        build 'test1-build'
      }
    }
    stage("deploy") {
      steps {
        build 'test1-deploy'
      }
    }
    stage("test") {
      steps {
        build 'test1-test'
      }
    }
  }
}
