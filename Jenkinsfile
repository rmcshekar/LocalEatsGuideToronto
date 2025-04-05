pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/rmcshekar/LocalEatsGuideToronto.git', branch: 'main'
            }
        }

        stage('List Files') {
            steps {
                sh 'ls -l'
            }
        }

        stage('Say Hello') {
            steps {
                echo 'Hello from LocalEatsGuideToronto pipeline!'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
