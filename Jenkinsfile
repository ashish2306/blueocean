pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''ls
pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'My name is Ashish'
          }
        }

        stage('test per') {
          steps {
            echo 'test per'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}