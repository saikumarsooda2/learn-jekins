pipeline {
    agent { node { label 'Workstation' } }

    environment {
    SSH = credentials('SSH')
    }
     options {
            ansiColor('xterm')
     }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh 'env'
            }
        }
    }

   post {
        always {
            echo 'I will always say Hello again!'
        }
    }
}