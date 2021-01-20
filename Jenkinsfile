node {
  try {
    stage('Test') {
      sh 'echo "Fail!"; exit 1'
    }
    echo 'This will run only if successful'
  } catch (e) {
      echo 'This will run only if failed'
      throw e 
  } finally {
      def currentResult = currentBuild.result ?: 'SUCCESS'
      if (currentResult == 'UNSTABLE') {
        echo 'This will run only if the run was marked as unstable'
      }

      def previousResult = currentBuild.previousBuild?.result
      if (previousResult != null && previousResult != currentResult) {
        echo 'This will run only if the state of the Pipeline has changed'
      }

      echo 'This will run always'
  }
}