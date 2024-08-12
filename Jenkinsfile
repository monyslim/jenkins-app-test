pipeline {
    agent any
    stages {
        stage('Set Permissions and Write') {
            steps {
                    sh '''
                        # Print the workspace directory for debugging
                        echo "Workspace directory: $WORKSPACE"

                        # Ensure the Jenkins user has the correct ownership of the workspace directory
                        echo "Changing ownership to ubuntu:jenkins..."
                        sudo chown -R ubuntu:jenkins /var/lib/jenkins/workspace/Freestyle

                        # Verify ownership
                        ls -ld $WORKSPACE

                        # change directory
                        cd /var/lib/jenkins/workspace/Freestyle

                        # Write to files in the workspace
                        echo "Test content" > /var/lib/jenkins/workspace/Freestyle/index.txt
                    '''
                }
            }
        }
    }
}
