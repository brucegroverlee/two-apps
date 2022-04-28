pipeline {
  agent any
  stages {
    stage('stage one') {
      agent {
        node { label 'nodejs' }
      }
      steps {
        sh 'node ./app-one/src/index.js'
      }
    }
  }
}