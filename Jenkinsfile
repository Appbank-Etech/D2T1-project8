pipeline{
    agent any
    stages{
        stage('1-git-clone by Mercy'){
            steps{
            checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Jenkin', url: 'https://github.com/Appbank-Etech/D2T1-project8.git']]]) 
            }
        } 
        stage('2-cpu check by Mercy'){
            steps{
                sh 'lscpu'
            }
        }
        stage('disk usage check by chris'){
            steps{
                sh 'du -h'
            }
        }
    }
}
