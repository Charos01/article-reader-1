pipeline {
    agent any 
    stages{
        stage('Initialize'){
            steps {
            
            sh '''
             ssh azureuser@20.16.79.71
            '''
            sh '''
             ansible-playbook Myplaybook.yml
            '''
             
             
            
            }
       }
      
    }
}

      

