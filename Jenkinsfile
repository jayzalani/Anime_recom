pipeline {
    agent any

    stages {
        stage("Cloning from GitHub") {
            steps {
                script {
                    echo 'Cloning from GitHub...'
                    checkout([$class: 'GitSCM',
                        branches: [[name: '*/main']],
                        userRemoteConfigs: [[
                            url: 'https://github.com/jayzalani/Anime_recom',
                            credentialsId: 'github-jenkins-token'
                        ]]
                    ])
                }
            }
        }
    }
}
