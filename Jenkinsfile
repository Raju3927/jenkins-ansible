 pipeline{
 agent any
 stages{
 stage('code checkout'){
  steps{
       git branch: 'main', url: 'https://github.com/Raju3927/jenkins-ansible.git'
       }
 }
 stage('Execute Ansible'){
  steps{
     ansiblePlaybook credentialsId: 'auser', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'dhost.inv', playbook: 'apache.yml' 
      }
    }
}
}
