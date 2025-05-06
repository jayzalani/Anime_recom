pipeline {
    agent any
    
    stages{
        stage("Clonning from Github....")
            steps{
                script{
                    echo 'Clonning from Github....'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-jenkins-token', url: 'https://github.com/jayzalani/Anime_recom']])
                }
            }
    }
}