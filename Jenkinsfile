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
    stage('PM2 install'){
      steps {
      sh "npm install pm2@latest -g"
      }
    }
    stage('Start application'){
      steps {
      sh "pm2 start server.js -f"
      }
    }
  }
}
