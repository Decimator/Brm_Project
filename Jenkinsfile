pipeline {
  agent any
  tools { 
      maven 'MAVEN_HOME' 
      jdk 'JAVA_HOME' 
    }
  stages {
    stage('hello') {
      steps {
        sh 'echo "Hello World"'
      }
    }
    stage('Build') {
        steps {
        sh 'mvn clean package'
      }
    }
  }
}
