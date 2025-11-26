pipeline{
    agent {label "server1"}

    stages{
        stage('build'){
            steps{
                bat 'mvn clean package'
            }

            post{
                success{
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }

    }
}