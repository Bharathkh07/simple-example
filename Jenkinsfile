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
                          sh 'mvn --version'
                    sh 'mvn clean validate'
                 }
                 }
                  stage('Docker') {
                           steps {
                                    sh 'docker --version '
                           }
                  }
              }
}
