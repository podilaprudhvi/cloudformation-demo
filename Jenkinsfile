pipeline {
    agent any
    environment {
    AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
    AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
   }
    stages {
        stage('Create Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket12 --template-body file://simplests3cft.json --region 'us-east-2'"
              }
            }
        }
     }
