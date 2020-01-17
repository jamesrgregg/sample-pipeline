pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }
    stages {
        stage('Check file') {
            steps {
                sh 'mkdir /tmp/ready'
                sh 'ls -hal /tmp'
                sh "cat /tmp/ready"
            }
        }
    }
}