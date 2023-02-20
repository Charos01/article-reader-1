pipeline {
    agent any
    stages {
        stage ("SCM checkout") {
            steps {
               sshagent(['mykey']) {
                  sh '''
                    ssh azureuser@20.251.50.253
                    ansible-playbook Myplaybook
                    '''

}
                
            }
        }
        stage ("checkout") {
            steps {
               sshagent(['mykey']) {
                  sh '''
                    pwd
                    /opt/kafka/kafka_2.13-3.3.1/bin/zookeeper-server-start.sh config/zookeeper.properties
                    '''

}
                
            }
        }
       
        

}
}




