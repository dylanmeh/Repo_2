pipeline {
  agent any

  tools{
    maven 'maven 3'
    jdk 'java 8'
  }
  stages {
    stage ("initialize") {
      steps {
        sh '''
        echo "PATH = ${PATH}"
        echo "M2_HOME = ${M2_HOME}"
        '''
      }
    }
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
