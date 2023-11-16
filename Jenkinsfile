pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }


 post {
    always {
     sh 'echo post'
    }
 }

