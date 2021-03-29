pipeline {
  agent any
  stages {
    

    

    stage('Code Analysis') {
      parallel {
        stage('Code Analysis') {
          steps {
            withSonarQubeEnv('sonarqube') {
              bat 'gradle sonarqube'
            }

          }
        }

        
      }
    }

    

   

  }
}