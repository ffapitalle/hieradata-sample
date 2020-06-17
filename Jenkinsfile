pipeline {
    agent {
        image 'cytopia/yamllint'
        args '-v $WORKSPACE:/data --entrypoint=/bin/ash'
    }
    stages {
        stage('Linter') {
            sh 'yamllint .'
        }
    }
}
