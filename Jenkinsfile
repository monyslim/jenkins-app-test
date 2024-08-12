pipeline {
    agent any
    stages {
        stage('Write and Verify') {
            steps {
                script {
                    sh '''
                        # Print the workspace directory for debugging
                        echo "Workspace directory: $WORKSPACE"

                        # Write to files in the workspace
                        echo "Test content" > $WORKSPACE/index.txt
                        echo "Hello World" > $WORKSPACE/taller.txt

                        # Output the contents of the files to verify
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
