pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Anmol346/onlinebookstore.git']])
                sh 'mvn clean install'          
            }
        }
    }
}
