pipeline {
  agent any

  triggers {
        cron('0 12,3,6 * * *')
  }
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }

      post {
        always {
        }
      }
    }
  }
}
