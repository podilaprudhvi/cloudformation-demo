pipeline {
    agent any
    environment {
    AWS_ACCESS_KEY_ID     = "jenkins-aws-secret-access-key"
    AWS_SECRET_ACCESS_KEY = "jenkins-aws-secret-key-id"
   }
    stages {
        stage('Create Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket13 --parameters ParameterKey=Applications,ParameterValue=1 --template-body file://simplests3cft.json --region 'us-east-1'"
              }
            }
        }
     }
