pipeline {
  agent {
    node {
      label 'myhost'
    }

  }
  stages {
    stage('Code Checkout') {
      steps {
        sh 'echo "Checking out code from github"'
      }
    }

    stage('Intallation') {
      steps {
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        sh 'ng lint'
      }
    }

    stage('Unit Tests') {
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