pipeline {
    agent {
        docker{
            image 'b00mgr3rt/micro-deployment:v1'
            args '--user root -v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                sh 'echo passed'
                git branch: 'main', url: 'https://github.com/bom254/microserving-testing.git'
            }
        }
    }
}