pipeline {
  agent any
  stages {
    stage('Code Analysis') {
      
          steps {
            withSonarQubeEnv('sonarqube') {
              bat 'gradle sonarqube'
            }

            waitForQualityGate true
          }
        
    }

  }
}