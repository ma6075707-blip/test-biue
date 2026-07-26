pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build commpleted'
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

    stage('deploy2') {
      steps {
        echo 'deploy4'
      }
    }

  }
}