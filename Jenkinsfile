pipeline {
    agent any
    
    
    stages{
        stage('Initialize'){
            steps {
            
            git branch: 'main', url: 'https://github.com/Charos01/article-reader-1'
            
            }
       }
        stage('Ansible'){
            steps { 
                ansiblePlaybook becomeUser: 'jenkins', installation: 'ansible', inventory: './hosts.yml', playbook: 'Myplaybook.yml'
            }
        }
        }

}
      

