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
      input {
        message "should we continue?"
        ok "we should"
      }
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