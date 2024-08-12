pipeline {
    agent any  // This allows the pipeline to run on any available Jenkins agent
    stages {
        stage('Setup') {
            steps {
                script {
                    // Running shell commands to create and modify files
                    sh '''
                        #!/bin/bash
                        echo "Welcome here" > $WORKSPACE/index.txt
                        echo "Current directory:"
                        pwd
                        echo "Hello World" > $WORKSPACE/taller.txt
                    '''
                }
            }
        }
    }
}