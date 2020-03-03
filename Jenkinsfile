pipeline {
  agent any
    stages {
      stage ('Build') {
        steps {
          withAWS(region: 'us-west-2', credentials: 'aws-static') {
            s3Upload(file: 'index.html', bucket: 'udacity-pipeline-project')
          }  
        }
      }
    }
}
