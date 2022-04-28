pipeline {
  agent any
  stages {
    stage('general stage') {
      steps {
        sh 'echo Hello General Stage'
      }
    }
    stage('stage app one') {
      when {
        changeset "app-one/**"
      }
      steps {
        sh 'echo app one got some changes'
      }
    }
    stage('stage app two') {
      when {
        changeset "app-two/**"
      }
      steps {
        sh 'echo app two got some changes'
      }
    }
    stage('stage app three') {
      when {
        changeset "app-three/**"
      }
      steps {
        sh 'echo app three got some changes'
      }
    }
  }
}