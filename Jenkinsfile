pipeline {
    agent any 
    stages{
        stage('Initialize'){
            steps {
            
            sh '''
             ssh azureuser@20.16.79.71
            '''
             sh '''
             sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible

sudo apt update
sudo apt install ansible
            '''
            sh '''
             ansible-playbook Myplaybook.yml
            '''
             
             
            
            }
       }
      
    }
}

      

