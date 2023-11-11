pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is bulid step'
          }
        }

        stage('send msg to dev') {
          steps {
            sh 'ls -h'
          }
        }

      }
    }

  }
}