@Library('dcube-library') _

pipeline {
    
    options {
      ansiColor('xterm') {
        // Just some echoes to show the ANSI color.
        stage "\u001B[31mI'm Red\u001B[0m Now not"
      }
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
