pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/lasharibaloch/angularproject', branch: 'main')
      }
    }

    stage('Build') {
      steps {
        sh 'ng build --prod'
      }
    }

  }
}