pipeline {
    agent any 
    stages{
        stage('Initialize'){
            steps {
            git branch: 'main', url: 'https://github.com/Charos01/article-reader-1'
            sh '''
             
             ssh azureuser@20.16.79.71
             ansible-playbook Myplaybook.yml
            '''
             sh '''
             whoami
            '''
           
             
            
            }
       }
       
      
    }
}

      

