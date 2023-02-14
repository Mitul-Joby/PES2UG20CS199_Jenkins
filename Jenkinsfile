pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES2UG20CS199 PES2UG20CS199.cpp'
        echo 'Build Successful'
      }
    }
    stage('Test') {
      steps {
        sh './PES2UG20CS199'
        echo 'Test Successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployment successful'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
