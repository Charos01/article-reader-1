pipeline {
    agent any
    stages{
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'Jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook', credentialsId: 'mykey'
            }
        }
        }
}


