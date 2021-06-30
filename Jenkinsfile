pipeline {
  agent agent1

  stages {
    stage ('preparing the Artifact') {
      steps{
       sh '''
         zip  -r  ../frontend.zip *
       '''
      }
    }
  }
}
