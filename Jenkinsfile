pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/shivang10ag/Crypto-Prediction', branch: 'master')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            powershell 'ls -Force'
          }
        }

        stage('Front -end Unit Tests ') {
          steps {
            powershell 'cd curriculum-front; npm install; npm run test:unit'
          }
        }

      }
    }

  }
}