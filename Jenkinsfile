pipeline {
    agent any 
    stages{
        stage('Initialize'){
            steps {
            
            sh '''
             ssh azureuser@20.16.79.71
            '''
             sh '''
             whoami
            '''
           
             
            
            }
       }
         stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'docker-playbook.yml', vaultCredentialsId: 'mykey'
            }
        }
      
    }
}

      

