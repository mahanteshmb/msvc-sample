pipeline {
  agent any
  stages {
    stage('Build User Service') {
      parallel {
        stage('Build User Service') {
          steps {
            echo 'Started Building User Service'
          }
        }
        stage('Build Front End') {
          steps {
            echo 'Starting to Build Front End'
          }
        }
      }
    }
    stage('Build Posts Service') {
      steps {
        echo 'Starting to Build Posts Service'
      }
    }
  }
}