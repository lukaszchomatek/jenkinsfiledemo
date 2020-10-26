pipeline {
    agent any
    environment {
        FOO = 'foo_env'
        DB_LOGIN = credentials('local-database')
    }
    stages {
        stage('Say hello') {
            environment {
                BAR = 'bar_env'
            }
            steps {
                echo 'Hello world from Git!'
                echo $DB_LOGIN
                sh 'printenv'
            }
        }
    }
}