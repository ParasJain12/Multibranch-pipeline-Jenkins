@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        //main branch
        //Hello
        stage('Hello') {
            steps {
                echo 'Hello, Jenkins!'
            }
        }
        stage('Use Common Library') {
            steps {
                script {
                    common.printMessage('Hello from shared library')
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    echo "Building branch ${env.BRANCH_NAME}"
                    if (env.BRANCH_NAME == 'main') {
                        echo "This is production"
                    } else {
                        echo "This is a feature branch"
                    }
                }
            }
        }
    }
}
