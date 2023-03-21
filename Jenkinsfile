pipeline {
  agent any
  stages {
    stage('Code Checkout') {
      steps {
        git(url: 'https://github.com/lasharibaloch/angularproject', branch: 'main')
      }
    }

    stage('build') {
      steps {
        sh 'ng build --prod'
      }
    }

  }
}