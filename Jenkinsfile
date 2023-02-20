pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
               sshagent(['mykey']) {
                  sh '''
                    ssh azure
                    ansible-playbook Myplaybook
                    '''

}
                
            }
        }
       
        

}
}




