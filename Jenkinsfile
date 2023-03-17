pipeline {
  agent {
    node {
      label 'myhost'
    }

  }
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/lasharibaloch/angularproject', branch: 'main')
      }
    }

    stage('Installation of nodejs') {
      steps {
        sh 'npm install '
      }
    }

    stage('Test') {
      steps {
        sh 'npm run test --watch=false'
      }
    }

    stage('Build') {
      steps {
        sh 'ng build --prod'
      }
    }

  }
}