pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
         echo "Hello World"
      }
    }
    stage('Test') {
    parallel {
      stage('Test On Windows') {
        steps {
          echo "Running tests on Windows"
        }
      }
      stage('Test On Linux') {
        steps {
          echo "Running tests on Linux"
        }
      }
    }
  }
