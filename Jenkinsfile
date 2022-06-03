pipeline{
    agent any
    stages{
        stage('git-clone by Mercy'){
            steps{
            checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Jenkin', url: 'https://github.com/Appbank-Etech/D2T1-project8.git']]]) 
            }
        } 
        stage('cpu check by Mercy'){
            steps{
                sh 'lscpu'
            }
        }
        stage('5-disk usage check by chris'){
            steps{
                sh 'du -h'
            }
        }
    }
}
