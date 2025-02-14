pipeline {
    agent { label 'agent_maven_1' }
    stages {
        stage('clone') {
            steps {
                git branch: 'main', url: 'https://github.com/manjushalanjewar7/java-war-repo.git'
            }
        }
        stage('Build') {
              steps {
                  sh 'mvn clean install'
              }
        }
    }
}
