pipeline {
    agent any
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook.yml', credentialsId: 'mykey'
            }
        }
        }


