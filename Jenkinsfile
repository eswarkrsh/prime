pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'date'
          }
        }
        stage('test') {
          steps {
            git(url: 'https://github.com/eswarkrsh/prime', poll: true)
          }
        }
      }
    }
  }
}