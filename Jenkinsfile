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
        stage('test') {
          steps {
            echo 'running test'
          }
        }

        

      }
    }

    

  }
}