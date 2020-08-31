pipeline {
  agent any
  stages {
    stage('prerequisite') {
      steps {
        bat 'git pull'
        bat 'npm install'
        bat 'npm test'
      }
    }

  }
}