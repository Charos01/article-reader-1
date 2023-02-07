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
               Ansible becomeUser: 'jenkins', credentialsId: 'mykey', installation: 'Ansible', playbook: 'Myplaybook.yml', sudo: true, sudoUser: null
            }    
        }    
    }
}

