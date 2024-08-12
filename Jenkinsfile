pipeline {
    agent any
    stages {
        stage('Write and Verify') {
            steps {
                script {
                    sh '''
                        echo "Welcome here" > $WORKSPACE/index.txt
                        echo "Hello World" > $WORKSPACE/taller.txt
                        echo "Contents of index.txt:"
                        cat $WORKSPACE/index.txt
                        echo "Contents of taller.txt:"
                        cat $WORKSPACE/taller.txt
                    '''
                }
            }
        }
    }
}
