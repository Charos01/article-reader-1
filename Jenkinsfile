pipeline {
    agent any
    stages{
       
        stage('Ansible'){
            steps { 
                ansiblePlaybook credentialsId: 'f242b5a9-9f11-4de5-8885-ed73d023a654', playbook:'Myplaybook'
                 
            }
        }
        }

}
