pipeline {
  agent any {
  stages {
    stage('build') {
      steps {
        sh 'echo " hai "'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo " test is triggerd"'
          }
        }
        stage('unit test') {
          steps {
            sh 'echo " unit test is triggered"'
          }
        }
        stage('integration test') {
          steps {
            sh 'echo " test is running"'
          }
        }
      }
    }
    stage('stagging area') {
      steps {
        sh 'echo " staging area is running"'
      }
    }
    stage('prod') {
      steps {
        sh 'echo " depoly prod"'
      }
    }
  }
}
