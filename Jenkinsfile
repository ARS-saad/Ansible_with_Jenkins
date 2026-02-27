pipeline {
  agent any
  stages {
    stage('Run Ansible') {
      steps {
        sshagent(['ubuntu (VE)']) {
            sh 'ansible-playbook -i hosts p1.yaml'
        }
      }
    }
  }
}
