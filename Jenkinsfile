pipeline {
    agent any
    stages {
        stage('Cloning code') {
            steps {
            
                git 'https://github.com/Preethi564/hello-world.git'

            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
                  }
        }
        stage('Secure Copy') {
            steps {
                sh 'sudo scp /var/lib/jenkins/workspace/Project-MBP_master/webapp/target/webapp.war root@ip-172-31-46-163:/opt/tomcat/apache-tomcat-10.1.6/Project-MBP-warfile'
           }
            
        }
    }
}
