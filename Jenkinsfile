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
            
          }
        )
      }
    }
    stage('Stage 2') {
      steps {
        sh 'mvn -v'
      }
    }
  }
}