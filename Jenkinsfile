pipeline {
  agent any
  tools {nodejs "node"}
  stages {
    
    stage('Cloning Git') {
      steps {
        git 'https://github.com/melivader/my-app-1'
      }
    }

    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
         sh 'npm test'
      }
    }
  }
}
