pipeline {
  agent any
  tools {
    nodejs 'node-11.0.0'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('Instar dependencias') {
      steps {
        sh 'npm i'
      }
    }
    stage('Run tests') {
      steps {
        sh 'npm test'
      }
    }
  }
}