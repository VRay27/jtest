pipeline {
  agent any
  stages {
    stage('New Branch Build') {
      steps {
        echo 'New branch build step'
        sh 'whoami'
      }
    }

    stage('New Branch Testing ') {
      steps {
        echo 'This is a testing stage'
        sh 'whoami'
      }
    }

    stage('New Branch Deploy') {
      steps {
        echo 'This is a depolying stage'
      }
    }

  }
}