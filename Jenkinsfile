pipeline {
  agent any
  stages {
    stage('Fluffy build') {
      steps {
        sh './jenkins/build.sh'
      }
    }
    stage('Fluffy test') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }
    stage('Fluffy deploy') {
      steps {
        sh ' ./jenkins/deploy.sh staging'
      }
    }
  }
}