pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/Amits64/jpetstore-6.git'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }
    stage('Deploy') {
      steps {
        sh 'cp target/jpetstore.war /opt/tomcat/webapps/'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing stage'
      }
    }

  }
}
