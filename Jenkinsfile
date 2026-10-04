pipeline {
    agent any

    stages {
        stage('Environment') {
            steps {
                sh 'echo $PATH'
                sh 'which mvn || true'
                sh 'which java || true'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn validate'
            }
        }

        stage('Hello') {
            steps {
                echo 'Hello from Jenkins!'
            }
        }
    }
}
