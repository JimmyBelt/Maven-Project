pipeline {
    agent {label "server1"}
    stages {
        stage('Checkout') {
            steps {
                withEnv(['GIT_SSH_COMMAND=C:\\Program Files\\Git\\usr\\bin\\ssh.exe -i C:\\Users\\jaime\\.ssh\\id_rsa -o StrictHostKeyChecking=no']) {
                    git url: 'ssh://git@github.com/JimmyBelt/Maven-Project.git', branch: 'main'
                }
            }
        }
    }
}
