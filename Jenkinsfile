
pipeline {
    agent any
    tools{
        maven "maven 3.5.0"
    }
    stages{   
stage('Email Notification'){
    mail bcc: '', body: '''Build successful!!!!
    Thanks,
    echo 'e-mail OK!'
}
        
                stage("verify tooling") {
             steps {
                sh '''
				
                  docker version
                  docker info
                  docker compose version 

                '''
				}
      }

        
          stage('docker-compose-microservices') {
           steps {
              sh "docker compose up -d"
		   
             
           }
       }

}
}
