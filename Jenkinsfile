pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Clone Repository') {
            steps {
                checkout scm
            }
        }

        stage('Print File Contents') {
            steps {
                script {
                    echo "====================="
                    echo "Content of final_test.txt:"
                    echo readFile('final_test.txt').trim()
                    echo "====================="

                    echo "Content of test.txt:"
                    echo readFile('test.txt').trim()
                    echo "====================="

                    echo "Content of test2.txt:"
                    echo readFile('test2.txt').trim()
                    echo "====================="
                }
            }
        }
    }
}
