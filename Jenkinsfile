pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Demo App'
        sh 'sh `mvn  compile` '
      }
    }

    stage('Test') {
      steps {
        echo 'Deliver'
        sh 'sh `./jenkins/scripts/deliver.sh`'
      }
    }

  }
}