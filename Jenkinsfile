pipeline {
  agent any
  stages {
    stage('Run Ansible') {
      steps {
        sshagent(['VE']) {
            sh 'ansible-playbook -i hosts p1.yaml'
        }
      }
    }
  }
}
