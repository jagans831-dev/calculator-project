
pipeline {
    agent any

    stages {

        stage('Welcome') {
            steps {
                echo 'Welcome to Calculator CI/CD!'
            }
        }

        stage('Checkout Verification') {
            steps {
                echo 'Checking Calculator source files...'

                sh 'test -f index.html'
                sh 'test -f style.css'
                sh 'test -f app.js'

                echo 'All source files found!'
            }
        }

        stage('Build Complete') {
            steps {
                echo 'Calculator CI pipeline completed!'
            }
        }
    }
}
