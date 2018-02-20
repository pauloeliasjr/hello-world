pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Pre-build') {
          steps {
            sh 'docker info'
          }
        }
        stage('Test') {
          steps {
            sh '''ls -l
'''
            fileExists 'Jenkinsfile'
          }
        }
      }
    }
    stage('Approval') {
      steps {
        input 'Voce aprova?'
      }
    }
  }
}