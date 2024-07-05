pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                echo "Welcome to Your first class using Jenkins"
            }
        }
        stage("Debugging: Check File and Directory") {
            steps {
                sh '''
                    if [ ! -d /home/cyclobold-computer-3/jenkins-app-test ]; then
                        echo "Creating directory"
                        mkdir -p /home/cyclobold-computer-3/jenkins-app-test
                    else
                        echo "Directory exists"
                    fi
                    
                    if [ ! -f /home/cyclobold-computer-3/jenkins-app-test/index.txt ]; then
                        echo "Creating file"
                        touch /home/cyclobold-computer-3/jenkins-app-test/index.txt
                    else
                        echo "File exists"
                    fi

                    echo "Testing write permissions"
                    echo "Testing write permissions" >> /home/cyclobold-computer-3/jenkins-app-test/index.txt
                    cat /home/cyclobold-computer-3/jenkins-app-test/index.txt
                '''
            }
        }
        stage("checkout something") {
            steps {
                sh '''
                    echo "Adding 'Welcome' to file"
                    echo "Welcome" >> /home/cyclobold-computer-3/jenkins-app-test/index.txt
                    cat /home/cyclobold-computer-3/jenkins-app-test/index.txt
                '''
            }
        }
        stage("rolling") {
            steps {
                sh '''
                    echo "Adding 'gotcha' to file"
                    echo "gotcha" >> /home/cyclobold-computer-3/jenkins-app-test/index.txt
                    cat /home/cyclobold-computer-3/jenkins-app-test/index.txt
                '''
            }
        }
    }
}
