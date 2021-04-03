pipeline {
         agent any
         stages {
                  stage('Checkout code') {
        steps {
            checkout scm
        }
    }
                 stage('One') {
                 steps {
                     echo 'Hi'
                 } 
                }
                 stage('Two') {
                 steps {
                    input('Do you want to proceed?')
                 }
                 }
              }
}
