pipeline {
  agent any
  stage('Run Ansible') {
    agent {
        docker { image 'willhallonline/ansible:latest' } 
    }
    steps {
        sshagent(['ubuntu (VE)']) {
            sh 'ansible-playbook -i hosts p1.yaml'
        }
    }
}
}
