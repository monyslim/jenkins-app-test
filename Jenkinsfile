pipeline {
    agent any
    stages {
        stage('Set Permissions and Write') {
            steps {
                script {
                    sh '''
                        # Define the full path to the workspace
                        FULL_PATH="/var/lib/jenkins/workspace/Freestyle"

                        # Print the full path for debugging
                        echo "Workspace directory: $FULL_PATH"

                        # Ensure the Jenkins user has the correct ownership of the workspace directory
                        echo "Changing ownership to ubuntu:jenkins..."
                        sudo chown -R ubuntu:jenkins $FULL_PATH

                        # Verify ownership
                        ls -ld $FULL_PATH

                        # Write to files in the workspace
                        echo "Test content" > $FULL_PATH/index.txt
                        echo "Hello World" > $FULL_PATH/taller.txt

                        # Output the contents of the files to verify
                        echo "Contents of index.txt:"
                        cat $FULL_PATH/index.txt

                        echo "Contents of taller.txt:"
                        cat $FULL_PATH/taller.txt
                    '''
                }
            }
        }
    }
}
