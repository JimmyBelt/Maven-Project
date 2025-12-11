pipeline {
    agent {label "server1"}
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
