pipeline {
  agent any
  stages {
    stage('Build User Service') {
      parallel {
        stage('Build User Service') {
          steps {
            echo 'Started Building User Service'
            dir(path: 'User-Service') {
              sh 'docker image build -t userservice:1.1-$BUILD_ID .'
            }

          }
        }
        stage('Build Front End') {
          steps {
            echo 'Starting to Build Front End'
            sh 'docker image build -t frontendservice:1.1-$BUILD_ID Front-End'
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