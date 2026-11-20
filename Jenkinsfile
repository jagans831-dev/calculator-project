
pipeline {
    agent any

    stages {

        stage('Welcome') {
            steps {
                echo 'Welcome to Calculator CI/CD!'
            }
        }

        stage('Check Source Files') {
            steps {
                echo 'Checking Calculator project files...'

                sh 'test -f index.html'
                sh 'test -f style.css'
                sh 'test -f app.js'

                echo 'All Calculator source files found!'
            }
        }

        stage('Check Dockerfile') {
            steps {
                sh 'test -f Dockerfile'
                echo 'Dockerfile found successfully!'
            }
        }

        stage('Build Complete') {
            steps {
                echo 'Calculator CI pipeline completed!'
            }
        }
    }
}