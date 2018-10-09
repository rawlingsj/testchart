pipeline {
    agent any
    stages {
      stage('CI Build and push snapshot') {
        when {
          branch 'PR-*'
        }
        steps {
          echo "in a PR"
        }
      }
      stage('Build Release') {
        when {
          branch 'master'
        }
        steps {
          echo "in master"
        }
      }
    }
  }
