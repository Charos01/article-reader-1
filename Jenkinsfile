pipeline {
    agent any
     tools {
        
         
         dockerTool 'docker'
         
         }
    
    stages{
       
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook'
            }
        }
        }

}
