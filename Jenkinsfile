pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Hello'
          }
        }

        stage('') {
          steps {
            ws(dir: '/')
          }
        }

      }
    }

    stage('hello') {
      agent {
        node {
          label 'node'
        }

      }
      steps {
        error 'try'
      }
    }

  }
}