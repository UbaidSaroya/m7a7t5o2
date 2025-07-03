pipeline {
    agent any
    environment {
        MY_SECRET = credentials('my-github-token')
    }
    stages {
        stage('Show Secret') {
            steps {
