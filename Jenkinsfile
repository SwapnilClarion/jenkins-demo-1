pipeline {
  agent any
  stages {
    stage('prerequisite') {
      parallel {
        stage('prerequisite') {
          steps {
            bat 'git pull'
            bat 'npm install'
          }
        }

        stage('Run tests') {
          steps {
            bat 'npm run test'
          }
        }

      }
    }

  }
}