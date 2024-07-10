pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                echo "Welcome to Your first class using Jenkins"
            }
        }
        stage("checkout something") {
            steps {
                sh '''
                    echo "Welcome" >> index.txt
                '''
            }
        }
        stage("rolling") {
            steps {
                sh '''
                    echo $HOME
                    pwd
                '''
            }
        }
    }
}
