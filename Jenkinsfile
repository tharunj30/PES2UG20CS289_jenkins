pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ jenk.cpp -o jenk'
      }
    }
    
    stage('Test') {
      steps {
        sh './jenk'k
      }
    }
    
    stage('Deploy') {
      steps {
        echo 'Deployed!'
      }
    }
  }
  
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
