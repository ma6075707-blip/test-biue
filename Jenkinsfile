pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build commpleted'
        retry(count: 3) {
          echo 'trying'
        }

      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'running test 1'
          }
        }

        stage('test2') {
          steps {
            echo 'print 2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment '
      }
    }

    stage('') {
      steps {
        echo 'trying'
        retry(count: 3) {
          echo 'trying'
        }

        sh 'rfhhhhhhh'
      }
    }

  }
}