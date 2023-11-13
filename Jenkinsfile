pipeline {
  agent any
  stages {
    stage('Step 1') {
      steps {
        sh 'echo \'Hi, GeekFlare. Starting to build the App.\''
      }
    }

    stage('Step 2') {
      steps {
        sh 'input(\'Do you want to proceed?\')'
      }
    }

    stage('Step 3') {
      steps {
        sh 'echo "Start the deploy ..."'
      }
    }

  }
}