pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date '''
      }
    }

    stage('testing') {
      parallel {
        stage('testing') {
          steps {
            echo 'teststap'
          }
        }

        stage('test_2') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}