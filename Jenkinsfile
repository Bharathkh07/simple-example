pipeline {
         agent any
         stages {
                  stage('Checkout code') {
        steps {
            checkout scm
        }
    }
                 stage('Build') {
                 steps {
                     sh 'mvn clean compile'
                 } 
                }
                 stage('Test') {
                 steps {
                    sh 'mvn clean validate'
                 }
                 }
              }
}
