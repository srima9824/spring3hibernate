pipeline {
         agent any
         stages {
                 stage('Build') 
                 {

                    steps {
                           sh 'mvn clean package'
                           sh 'cd /etc/ansible'
                           sh 'ansible-playbook deploywar.yml'      
                          }
                 }
                }
}
