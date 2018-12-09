pipeline {
  agent any
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            echo 'HI - First step in pipeline'
          }
        }
        stage('checkout_parallel') {
          steps {
            sh 'maven clean compile'
          }
        }
      }
    }
  }
}