pipeline {
    agent any
    stages{
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'azureuser', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook.yml', credentialsId: 'mykey'
            }
        }
        }
}


