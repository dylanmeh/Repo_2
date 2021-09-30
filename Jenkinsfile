pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        sh returnStatus: true, script: '''npm install'''
      }
    }
    /** stage ('test') {
      steps {
        sh ''
      }
    }
    stage ('deploy') {
      steps {
        sh ''
      }
    } **/
  }
}  
