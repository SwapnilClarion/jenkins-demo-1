pipeline {
  agent any
  stages {
    stage('prerequisite') {
      parallel {
        stage('prerequisite') {
          steps {
            bat 'git pull'
            bat 'npm install'
            bat 'npm run test'
          }
        }

        stage('Demo stage') {
          steps {
            bat 'npm run test'
          }
        }

      }
    }

  }
}