pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build 'test1_build'
      }
    }
    stage('Deploy') {
      steps {
        build 'test1_deploy'
      }
    }
    stage('Test') {
      steps {
        build 'test1_test'
      }
    }
  }
}