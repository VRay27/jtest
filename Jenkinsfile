pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'This is a building stage'
          }
        }

        stage('buil2') {
          steps {
            echo 'Build 2 new message from the blue ocean editor'
            sh 'echo whoami'
          }
        }

      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'This is a testing stage'
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