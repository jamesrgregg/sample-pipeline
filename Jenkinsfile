pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
            args '--entrypoint='
        }
    }
    stages {
        stage('Check file') {
            steps {
                sh 'mkdir /tmp/ready'
                sh 'ls -hal /tmp'
                sh 'echo "test" > /tmp/ready/test'
                sh "cat /tmp/ready/test"
            }
        }
    }
}