pipeline {
  agent any
  environment {
    NODE_NAME = 'tula_mulava'
  }
  stages {
    stage('Build') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        echo "This is Java path: ${env.JAVA_HOME}"
        echo "Node name is ${env.NODE_NAME}"
        echo "This is workspace: ${env.WORKSPACE}"
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