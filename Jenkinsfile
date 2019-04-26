pipeline {
  agent any
  stages {
    stage('test1_build') {
      steps {
        build 'test1_build'
      }
    }
    stage('test1_deploy') {
      steps {
        build 'test1_deploy'
      }
    }
    stage('test1_test') {
      stpes{
        build 'test1_test'
      }
    }
  }
}
