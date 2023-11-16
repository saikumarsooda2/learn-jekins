pipeline {
    agent { node { label 'Workstation' } }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }

   post {
        always {
            echo 'I will always say Hello again!'
        }
    }
}