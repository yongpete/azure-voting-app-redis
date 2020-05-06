pipeline {
  agent any
  stages {
    stage('Echo on master') {
      when { branch 'master' }
      steps {
        echo 'This is the master branch'
      }
    }
  }
}