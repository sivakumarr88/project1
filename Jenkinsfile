pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'hello'
            }
        }

        stage('feature') {
            when {
                branch 'feature/*'
            }
            steps {
                echo 'Running feature branch stages'
            }
        }

        stage('main') {
            when {
                branch 'main'
            }
            steps {
                echo 'Running main branch stages'
            }
        }
    }
}