pipeline {
   agent any
      stages {
         stage('Clone Repository') {
            steps {
               git 'https://github.com/oramoetaro/jenkins_test.git'
            }
         }
         stage('Install Dependencies') {
            steps {
               sh 'npm install'
            }
         }
         stage('Build') {
            steps {
               sh 'npm run build'
            }
         }
         stage('Test') {
            steps {
               sh 'npm test'
            }
         }
      }
}

