pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Repository cloned by Jenkins'
            }
        }

        stage('Run Script') {
            steps {
                sh './app.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline finished successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}

