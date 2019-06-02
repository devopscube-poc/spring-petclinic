
pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {             
                gitCheckout(
                      url: 'https://github.com/devopscube-poc/spring-petclinic.git',
                      version: 'master'
                  )               
            }
        }
    }
}
