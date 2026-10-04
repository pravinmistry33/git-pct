pipeline {
    agent any

    tools {
        maven 'Maven-3.10'
    }

    stages {
        stage('Build & Test') {
            steps {
                sh 'mvn clean test'
            }

            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }

        stage('Hello') {
            steps {
                echo 'Hello from Jenkins!'
            }
        }
    }
}
