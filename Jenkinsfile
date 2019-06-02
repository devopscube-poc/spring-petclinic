@Library('dcube-library') _

pipeline {
    agent any

    stages {
        stage("Authorize Pipeline") {
            input {
              message 'TESTING'
              submitter 'testuser'
              parameters {
              text defaultValue: 'dev', description: '', name: 'ENV'
              text defaultValue: 'dev-cluster', description: '', name: 'CLUSTER'
              }
            }            
        }
        stage('Git Checkout') {
            steps {             
                gitCheckout(
                      url: 'https://github.com/devopscube-poc/spring-petclinic.git',
                      branch: 'master'
                  )               
            }
        }
    }
}
