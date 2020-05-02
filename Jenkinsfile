pipeline{
  agent any
  stages {
    stage('Upload to AWS'){
      withAWS(region:'eu-east-2',credentials:'aws-static',) {
          s3Upload(file:'index.html', bucket:'mina-jenkins-project', path:'./index.html')
      }
    }
  }
}