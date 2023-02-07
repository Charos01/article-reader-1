pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
               sshagent(['mykey']) {
                  sh '''
                    ssh azureuser@20.16.79.71 
                    ansible-playbook Myplaybook.yml
                    '''

}
                
            }
        }
       
        

}




