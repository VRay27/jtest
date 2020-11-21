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

    stage('test') {
      parallel {
        stage('Testing 1') {
          steps {
            echo 'This is a testing stage'
            sh 'whoami'
          }
        }

        stage('Testing 2') {
          steps {
            build 'Test2'
            sh 'echo "Testing started"'
            echo 'test completed'
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