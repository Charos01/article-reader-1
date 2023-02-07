pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
                git "https://github.com/Charos01/article-reader-1.git"
                
            }
        }
        stage(" execute Ansible") {
           steps {
                ansiblePlaybook credentialsId: 'mykey', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.yml', playbook: 'Myplaybook.yml'
            }    
        }    
    }
}

