pipeline {
    agent any 
    stages{
        stage('Initialize'){
            steps {
            
            sh '''
             ssh azureuser@20.16.79.71
            '''
             
             
            
            }
       }
        stage('Ansible'){
            steps { 
                ansiblePlaybook become: true, installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook.yml'
                
            }
    }
    }
}

      

