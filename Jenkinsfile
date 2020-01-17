pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }
    stages {
        stage('Check file') {
            steps {
                sh 'ls -hal /tmp'
                sh "cat /tmp/ready"
            }
        }
    }
}