pipeline {
    agent any
    stages {
      stage('CI Build and push snapshot') {
        when {
          branch 'PR-*'
        }
        steps {
	  sh 'env | sort'
          echo "in a PR"
        }
      }
      stage('Build Release') {
        when {
          branch 'master'
        }
        steps {
          sh 'env | sort'
          echo "in master"
        }
      }
    }
  }
