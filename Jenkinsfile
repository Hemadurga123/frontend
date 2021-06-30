pipeline {
  agent any

  stages {
    stage ('preparing the Artifact') {
      steps{
       sh '''
         Zip -r ../frontend.zip *
       '''
      }
    }
  }
}
