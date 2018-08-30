pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('hello') {
            steps {
                sh 'echo hello'
            }
        }
        stage('Sanity check') {
            steps {
                input "are you ok?"
            }
        }

        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
