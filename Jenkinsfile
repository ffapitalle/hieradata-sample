pipeline {
    agent {
        docker {
            image 'cytopia/yamllint'
            args '-v $WORKSPACE:/data --entrypoint=/bin/ash'
        }
    }
    stages {
        stage('Linter') {
            steps {
                sh 'yamllint .'
            }
        }
    }
}
