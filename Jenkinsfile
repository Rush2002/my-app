pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                bat 'mvn clean install'
            }
        }
    }

    post {
        success {
            echo "Build succeeded!"
        }
        failure {
            echo "Build failed!"
        }
    }
}
