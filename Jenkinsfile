pipeline {
  agent any

  stages {

    stage('Checkout') {
      steps {
        git branch: 'develop', url: 'https://github.com/ahmadirfansyah/CodeIgniter.git'
      }
    }

    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }
  }

  post {
    success {
      echo 'Pipeline completed successfully!'
    }
    failure {
      echo 'Pipeline failed!'
    }
  }
}
