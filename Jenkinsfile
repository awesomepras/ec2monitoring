pipeline {
  agent none

  stages {
    stage('Deploy to Sharing Account') {
      agent {
        node {
          label 'alpine'
        }
      }
      steps {
        println "Deploying..."
        sh "aws cloudformation deploy --template-file ec2monitor.yaml --stack-name ${params.Account}-${params.Environment}-newinstance --region us-east-1 --parameter-overrides Environment=${params.Environment}  Account=${params.Account}  InstanceType=${params.InstanceType} --tags Account=${params.Account} Env=${params.Environment} Owner=TeamDynamite --capabilities CAPABILITY_NAMED_IAM --no-fail-on-empty-changeset"

      }
      post {
        success {
          println "Success! Ec2 instance created"
        }
        failure {
          println "Failed"
        }
        aborted {
          println "Job aborted. "
        }
      }
    }
 


  }
}
