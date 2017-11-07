pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I am building some code--Updated!'
      }
    }
    stage('Test') {
      parallel {
        stage('Unit Tests') {
          steps {
            echo 'Unit Tests Are Awesome!'
          }
        }
        stage('Integration Tests') {
          steps {
            echo 'Integration Tests Are Awesome!'
          }
        }
        stage('Smoke Tests') {
          steps {
            echo 'Where There is Smoke there is Fire!!!'
          }
        }
        stage('Reg Test') {
          steps {
            echo 'Reg Test executed'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Ship It!'
      }
    }
  }
}