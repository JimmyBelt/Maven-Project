pipeline{
    agent {label "server1"}

    tools{
        maven 'mymaven'
    }

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