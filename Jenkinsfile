pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
          sh 'mvn clean package'
      }
    }
    stage ('test') {
      steps {
        sh 'mvn test'
      }
    }
    stage ('deploy') {
      steps {
        sh 'mvn exec:java'
      }
    }
  }
}  
