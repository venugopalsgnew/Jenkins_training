pipeline {
    agent any 
    stages {
        stage('Git Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'Github_ID_TOKEN_LATEST', url: 'https://github.com/venugopalsgnew/Jenkins_training.git']])
            }

        }


    }
    
    
}