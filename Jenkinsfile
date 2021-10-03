pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
          mvn 'clean package'
      }
    }
    stage ('test') {
      steps {
        mvn 'test'
      }
    }
    stage ('deploy') {
      steps {
        sh 'mvn exec:java'
      }
    }
  }
}  
