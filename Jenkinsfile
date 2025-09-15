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
    }
}
