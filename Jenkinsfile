pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
               sshagent(['mykey']) {
                  sh '''
                    ssh azureuser@20.16.79.71 '''

}
                
            }
        }
        stage('Ansible'){
            steps { 
                 ansiblePlaybook become: true, becomeUser: 'jenkins', colorized: true, credentialsId: 'mykey', installation: 'Ansible', inventory: 'hosts.yml', playbook: 'Myplaybook.yml', sudo: true
            }
        
    }
}
}




