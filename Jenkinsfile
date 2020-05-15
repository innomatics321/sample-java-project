pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/innomatics321/sample-java-project.git', branch: 'master')
      }
    }

    stage('compile') {
      steps {
        bat 'mvn clean compile'
      }
    }

  }
  environment {
    dev = 'develop'
  }
}