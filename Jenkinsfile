pipeline {
  agent any
  stages {
    stage('NPM Install ') {
      steps {
        sh 'npm install'
      }
    }
    stage('NPM Test') {
      steps {
        sh 'npm test'
        echo 'Running Test'
      }
    }
    stage('NPM Start') {
      steps {
        sh 'npm start'
        echo 'Starting the app'
      }
    }
  }
}