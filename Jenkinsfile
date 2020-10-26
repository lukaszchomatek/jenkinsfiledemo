pipeline {
    agent any
    environment {
        FOO = 'foo_env'
    }
    stages {
        stage('Say hello') {
            environment {
                BAR = 'bar_env'
            }
            steps {
                echo 'Hello world from Git!'
                sh 'printenv'
            }
        }
    }
}