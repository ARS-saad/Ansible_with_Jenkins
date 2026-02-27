pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        //git 'https://github.com/devopssteps/day26.git'
        echo 'test'
      }
    }
    stage('Run Ansible') {
      steps {
        sshagent(['VE']) {
            sh 'ansible-playbook -i hosts p1.yaml'
            //sh 'ssh -o StrictHostKeyChecking=no ubuntu@54.221.103.118 "echo Connected from Jenkins!"'
        }  
      }
    }
  }
}
