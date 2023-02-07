pipeline {
    agent any
    stages{
       
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook'
            }
        }
        }

}
