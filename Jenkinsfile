pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
      }
    }

    stage('Test') {
      steps {
        echo 'Testing'
      }
    }

    stage('Deployment') {
      steps {
        echo 'Deploying 1'
      }
    }

  }
}