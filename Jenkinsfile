pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile.build'
            args '-v $WORKSPACE:/yaml'
        }
    }
    stages {
        stage('Linter') {
            steps {
                sh 'yamllint --no-warnings .'
            }
        }
    }
}
