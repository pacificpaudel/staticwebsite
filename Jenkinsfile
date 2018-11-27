pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build success'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test success'
          }
        }
        stage('platform 1-A') {
          steps {
            echo '1A'
          }
        }
        stage('Platform 2-A') {
          steps {
            echo '2A'
          }
        }
        stage('Platform 3-A') {
          steps {
            echo '3A'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy success'
      }
    }
  }
  environment {
    date = '1234'
  }
}