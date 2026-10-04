pipeline {
    agent any

    tools {
        maven 'Maven-3.10'
    }

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
