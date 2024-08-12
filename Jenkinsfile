pipeline {
    agent any
    stages {
        stage('Write and Verify') {
            steps {
                script {
                    sh '''
                        sudo -u jenkins bash
                        echo "Test content" > /var/lib/jenkins/workspace/Freestyle/index.txt
                        echo "Hello World" >  /var/lib/jenkins/workspace/Freestyle/testfile.txt
                        cat /var/lib/jenkins/workspace/Freestyle/index.txt
                        echo "Contents of taller.txt:"
                        cat $WORKSPACE/taller.txt
                    '''
                }
            }
        }
    }
}
