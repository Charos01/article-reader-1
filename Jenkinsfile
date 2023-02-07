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
                ansiblePlaybook become: true, credentialsId: 'mykey', installation: 'Ansible', playbook: '/var/lib/jenkins/workspace/Broker/Myplaybook.yml', sudo: true
            }
        }
        }

}
      

