pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                echo "Welcome to Your first Multibranch Jenkins-class"
            }
        }
        stage("checkout something") {
            steps {
                sh '''
                    cd /var/lib/jenkins/workspace/Freestyle
                    sudo chown -R jenkins:jenkins /var/lib/jenkins/workspace/Freestyle
                    sudo chmod -R 755 /var/lib/jenkins/workspace/Freestyle
                    sudo echo "Welcome" > index.txt
                '''
            }
        }
    }
}
