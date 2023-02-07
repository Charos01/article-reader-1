pipeline {
    agent any 
    stages{
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook',credentialsId: 'f242b5a9-9f11-4de5-8885-ed73d023a654'
            }
        }
        }

}
