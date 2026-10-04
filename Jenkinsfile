pipeline {
    agent any

    stages {
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
