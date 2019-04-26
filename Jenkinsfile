pipeline {
  agent any
  stages {
    stage('test1_build') {
      steps {
        build job: 'test1_build'
      }
    }
    stage('test1_deploy') {
      steps {
        build job: 'test1_deploy'
      }
    }
    stage('test1_test') {
      steps {
        build job: 'test1_test'
      }
    }
  }
}
