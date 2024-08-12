pipeline {
    agent any
    stages {
        stage('Debug') {
            steps {
                script {
                    sh '''
                        echo "Workspace: $WORKSPACE"
                        echo "Current user: $(whoami)"
                        echo "Current directory:"
                        pwd
                        echo "Files in workspace:"
                        ls -l $WORKSPACE
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
