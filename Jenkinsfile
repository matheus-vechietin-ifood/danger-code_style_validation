pipeline {
  agent any
  stages {
    stage('Preparar Ambiente') {
      steps {
        sh 'echo "AMBIENTE"'
      }
    }
    stage('Testes Unitários') {
      parallel {
        stage('Testes Unitários') {
          steps {
            sh 'echo "UNIT TEST"'
          }
        }
        stage('Testes de UI') {
          steps {
            sh 'echo "UI TEST"'
          }
        }
      }
    }
    stage('Gerar Build') {
      steps {
        sh 'echo "GENERATE IPA"'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "DEPLOY STAGE"'
      }
    }
    stage('Build Info') {
      steps {
        sh 'echo "INFO"'
      }
    }
  }
}