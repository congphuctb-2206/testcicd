pipeline {
    agent any
    stages {
        stage('SSH to EC2 Web') {
            steps {
                sshagent(credentials: ['web-server-ssh']) {
                    sh 'ssh -o StrictHostKeyChecking=no ubuntu@54.151.180.190 "echo Hello-World"'
                }
            }
        }
    }
}
