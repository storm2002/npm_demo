pipeline {
  agent {
    node {
      label 'node0'
    }
  }
  stages {
    stage('Install Dep') {
        steps {
          sh "npm install"
          }
        }
    stage('Run Test'){
      steps {
      sh "npm test"
      }
    }
    stage('Build'){
      steps {
      sh "npm run build"
      }
    }
    stage('Start application'){
      steps {
      sh "npm start"
      }
    }
  }
}
