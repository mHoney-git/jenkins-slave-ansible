pipeline {
    agent any 
    stages {
        stage ('installing jenkins on jenkins-slave-ansible instance') {
            steps {
                ansiblePlaybook credentialsId: 'AWS-SSH-KEY', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'site.yml'
              }
        }
    }
}