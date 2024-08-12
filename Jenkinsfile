pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                echo "Welcome to Your first normal branch Jenkins-class"
            }
        }
        stage("checkout something") {
            steps {
                sh '''
                    echo "Welcome" > /var/lib/jenkins/workspace/Freestyle/index.txt
                '''
            }
        }
        stage("rolling") {
            steps {
                sh '''
                    echo $HOME
                    pwd
                    echo "Hello World" /var/lib/jenkins/workspace/Freestyle/taller.txt
                '''
            }
        }
    }
}
