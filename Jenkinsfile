pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                sshagent(['jenkins_ssh_credential_id']) {
                    git url: 'ssh://git@github.com/JimmyBelt/Maven-Project.git', branch: 'main'
                }
            }
        }
    }
}
