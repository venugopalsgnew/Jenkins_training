pipeline {
    agent any 
    tools {
        maven 'Maven'
    }
    stages {
        stage('Git Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'Github_ID_TOKEN_LATEST', url: 'https://github.com/venugopalsgnew/Jenkins_training.git']])
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
       stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        


    }
    
    
}