pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Pre-build') {
          steps {
            sh 'docker info'
            fileExists 'Dockerfile'
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