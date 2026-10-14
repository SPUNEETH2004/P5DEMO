pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Java Program...'
                bat 'javac Hello.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Java Program...'
                bat 'java Hello'
            }
        }

        stage('Archive') {
            steps {
                echo 'Archiving Java Class File...'
                archiveArtifacts artifacts: '*.class'
            }
        }
    }
}
