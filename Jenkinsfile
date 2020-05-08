pipeline {

    agent any
    tools {
        maven 'maven_3_6_3'
    }
    stages {

         stage('Checkout Code from Git') {
               steps {
        git 'https://github.com/foreverankit/petclinic-tests.git'
    }}

    stage('compile stage') {
             steps {
                bat "mvn clean compile"
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

  }

}