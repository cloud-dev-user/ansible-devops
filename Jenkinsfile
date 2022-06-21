pipeline {
  agent any
  stages {
    stage('install tomcat ') {
      steps {
        sh 'ansible-playbook tomcat_install.yaml'
      }
    }

  }
}