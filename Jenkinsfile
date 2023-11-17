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
        parameters {
        string(name: 'PERSON', defaultValue: 'Enter Your Name please', description: 'Hello Mr shall we run')
        }
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