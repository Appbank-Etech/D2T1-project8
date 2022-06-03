Pipeline{
    Agent any
    Stages{
        Stage('git-clone'){
            Steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'c6cc7d2f-a647-4055-b461-69cd231119bd', url: 'https://github.com/Appbank-Etech/D2T1-project8.git']]])   
            }
        } 
    }
}