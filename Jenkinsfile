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
        string(name: 'PERSON', defaultValue: 'Mr.SAI KUMAR SOODA', description: 'Who I say Hello?')
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