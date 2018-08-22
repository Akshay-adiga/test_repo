pipeline {
  agent any

  triggers {
        cron('0 12,3,6 * * *')
  }
    
  tools {nodejs}
    
  stages {
        
    stage('Install dependencies') {

      steps {
        sh 'npm install'
      }

      post {
        always {
            mail to: 'akshaya.adiga@cognitiveclouds.com',
                 subject: "Test email Pipeline: ${currentBuild.fullDisplayName}",
                 body: "More Info: ${env.BUILD_URL}"
        }
      }
    }     
  }
}
