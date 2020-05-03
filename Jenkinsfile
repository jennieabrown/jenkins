pipeline {
environment {
  ucdApp = ${APP}
}
agent any

stages {
    stage('doBuildStuff') {
        steps {
           echo "build it here for ${ucdApp}"
         }
    }
    stage('runUCD'){
      steps {
        bat "ucd/showProps.cmd ${ucdApp}"
      }
    }
    stage('package'){
      steps{
       echo "do something more..."
      }
    }
  }
}
