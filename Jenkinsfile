pipeline {
    agent any

    parameters {
        choice(name: 'branch',
                choices: ['master'],
                description: 'Select the branch to clone'
                )
    }
    stages {
        stage('Clone repo') {
            steps {
                git branch: "${params.branch}", 
                credentialsId: '949e6469-3762-4c97-9949-4705f09cd426',
                url: 'https://github.com/Wei-Xiang2359/-BigBucks-Secret-Internet-Surveillance-Monitoring-Server.git'
            }
        }
    }
}
