pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
               git branch: 'main', url: 'https://github.com/Charos01/article-reader-1'
                
            }
        }
        stage(" execute Ansible") {
           steps {
                ansiblePlaybook credentialsId: 'mykey', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.yml', playbook: 'Myplaybook.yml'
            }    
        }    
    }
}

