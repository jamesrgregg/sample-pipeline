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
                echo "test" > test
                sh "cat /tmp/ready/test"
            }
        }
    }
}