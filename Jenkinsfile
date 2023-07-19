pipeline {
  agent {label 'slave-x1'}
  options { disableConcurrentBuilds() }
  stages {
    stage('test') {
        steps{
            sh 'ls -la'
        }
    }
  }
}