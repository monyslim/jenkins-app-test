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
                    echo "Welcome" >> /home/cyclobold-computer-3/jenkins-app-test/index.txt
                '''
            }
        }
        stage("rolling") {
            steps {
                sh '''
                    echo "gotcha" >> /home/cyclobold-computer-3/jenkins-app-test/index.txt
                    cat /home/cyclobold-computer-3/jenkins-app-test/index.txt
                '''
            }
        }
    }
}
