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
                sh 'sudo scp /var/lib/jenkins/workspace/Muiltibranch_Pipeline-Mini_dev/webapp/target/webapp.war /opt/mytomcat/apache-tomcat-10.1.6/MultiB-pipeline-warfile'
           }
            
        }
    }
}
