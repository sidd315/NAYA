pipeline {
  agent any
  stages {
    stage('BUILD') {
      parallel {
        stage('BUILD') {
          steps {
            bat 'echo %Name%'
          }
        }
        stage('Build2') {
          steps {
            bat 'echo "This is build2"'
          }
        }
      }
    }
    stage('Test') {
      steps {
        bat 'echo "Test"'
      }
    }
  }
  environment {
    Name = 'Sidd'
  }
}