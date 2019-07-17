pipeline {
         agent any
         stages {
                 stage('Build') 
                 {

                    steps {
                           sh 'mvn clean package'
                           sh 'ansible-playbook /etc/ansible/deploywar.yml -i /etc/ansible/hosts'      
                          }
                 }
                }
}
