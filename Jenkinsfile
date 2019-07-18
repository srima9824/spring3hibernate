pipeline {
         agent any
         stages {
                 stage('Build') 
                 {

                    steps {
                           sh 'mvn clean package'
                          }
                 }
                 stage('Deploy')
                 {
                   steps {
                          sh 'ansible-playbook /etc/ansible/deploywar.yml'
                         }
                 }

                }
}
