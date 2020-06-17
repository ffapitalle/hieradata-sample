pipeline {
    agent {
        docker {
            image 'sdesbure/yamllint'
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
