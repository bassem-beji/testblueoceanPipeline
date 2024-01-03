pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
      }
    }

    stage('teststages') {
      parallel {
        stage('test2') {
          steps {
            echo 'running test2'
          }
        }

        stage('test1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        input(message: 'are you sure to deploy', ok: 'yes, i am sure')
        echo 'deployment completed'
      }
    }

  }
}