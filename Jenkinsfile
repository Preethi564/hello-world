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
      }
    }


