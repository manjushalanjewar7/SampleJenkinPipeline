pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/manjushalanjewar7/java-war-repo.git'
            }
        }
        stage('Parallel Execution') {
            parallel {
                stage ('Build') {
              steps {
                  echo 'Building the Project...'
                  sh 'mvn clean install'
              }
           }
         stage('Test') {
             steps {
                 echo 'Running steps...'
         }
       }
     }
   }            
 }            
}    
            
