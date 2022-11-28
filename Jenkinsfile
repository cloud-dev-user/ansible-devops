pipeline {
  agent any
  stages {
    stage('install tomcat ') {
      steps {
        sh "ansible-playbook tomcat_install.yaml -e host_group=$ansible_env"
      }
    }

    stage('echo ') {
      steps {
        sh '''echo 

"hello world " '''
      }
    }

  }
  parameters {
    choice(name: 'ansible_env', choices: ['dev', 'test', 'uat'], description: 'this is environment to provided for ansible playbook variable: host_group')
  }
}