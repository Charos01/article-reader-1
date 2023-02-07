pipeline {
    agent any
    stages{
        stage('Initialize'){
            steps {
            
            sh '''
            ssh azure
            '''
             sh '''
             ansible-playbook Myplaybook
             
             '''
             sh '''
             whoami
             
             '''
            
            }
       }
    }
}
   
