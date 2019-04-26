pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        build 'test1_build'
      }
    }
    stage("deploy") {
      steps {
        build 'test1_deploy'
      }
    }
    stage("test") {
      steps {
        build 'test1_test'
      }
    }
  }
}
