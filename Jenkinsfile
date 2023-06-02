pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'parallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('Cleanup') {
      steps {
        echo 'cleaning'
      }
    }

  }
}