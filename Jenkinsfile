@Library('dcube-library') _

pipeline {
    
    options {
      ansiColor('xterm')
    }
    
    agent any

    stages {
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
