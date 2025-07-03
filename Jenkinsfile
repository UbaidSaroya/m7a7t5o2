pipeline {
    agent any

    triggers {
        githubPush()   // webhook trigger
    }

    stages {
        stage('Clone Repository') {
            steps {
                // Git clone karne ke liye checkout scm use karo
                checkout scm
            }
        }

        stage('Print Files Content') {
            steps {
                script {
                   
                    echo "===== test.txt ====="
                    echo readFile('test.txt')

                    echo "===== test2.txt ====="
                    echo readFile('test2.txt')

                    echo "===== final_test.txt ====="
                    echo readFile('final_test.txt')

                }
            }
        }
    }
}
