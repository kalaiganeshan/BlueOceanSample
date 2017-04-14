pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        parallel(
          "Print Hello": {
            echo 'Hello!'
            
          },
          "In Parallel": {
            echo 'Hello in parallel!'
            
          },
          "Parallel 3": {
            echo 'Hello!!!'
            
          }
        )
      }
    }
    stage('Stage 2') {
      steps {
        echo 'Hello again!'
      }
    }
  }
}