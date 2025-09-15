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

        stage('Feature Stage') {
            steps {
                echo 'This is the feature-1 branch!'
            }
        }

        stage('Use Common Library') {
            steps {
                script {
                    common.printMessage('Hello from shared library')
                }
            }
        }
    }
}
