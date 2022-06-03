pipeline{
    agent any
    stages{
        stage('git-clone'){
            steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'c6cc7d2f-a647-4055-b461-69cd231119bd', url: 'https://github.com/Appbank-Etech/D2T1-project8.git']]])   
            }
        } 
        stage('cpu check'){
            steps{
                sh 'lscpu'
            }
        }
    }
}
