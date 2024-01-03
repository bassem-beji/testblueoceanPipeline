pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
        retry(count: 3) {
          sh 'wwww'
        }

      }
    }

    stage('teststages') {
      parallel {
        stage('test') {
          steps {
            echo 'running test'
          }
        }

        

      }
    }

    

  }
}