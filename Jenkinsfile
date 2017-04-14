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
            echo 'Hello!'
            
          }
        )
      }
    }
  }
}