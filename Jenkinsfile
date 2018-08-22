pipeline {
  agent any

  triggers {
        cron('0 12,3,6 * * *')
  }
    
  
    
  stages {
        
    stage('Install dependencies') {

      steps {
        sh 'npm install'
      }

      
    }     
  }
}
