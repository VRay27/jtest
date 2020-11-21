pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('Build 1') {
          steps {
            echo 'This is a building stage'
          }
        }

        stage('Build 2') {
          steps {
            echo 'Build 2 new message from the blue ocean editor'
            sh 'whoami'
          }
        }

      }
    }

    stage('Testing 1') {
      parallel {
        stage('Testing 1') {
          steps {
            echo 'This is a testing stage'
            sh 'whoami'
          }
        }

        stage('Testing2') {
          steps {
            sh 'whoami'
            echo 'Hello from test2 '
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'This is a depolying stage'
      }
    }

  }
}