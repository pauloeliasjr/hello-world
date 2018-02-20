pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'pwd'
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
  }
}