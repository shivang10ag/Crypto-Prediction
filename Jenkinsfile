pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/shivang10ag/Crypto-Prediction', branch: 'master')
      }
    }

    stage('error') {
      steps {
        powershell 'ls -Force'
      }
    }

  }
}