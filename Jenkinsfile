pipeline {
        agent none
        stages {
         
          stage("build & SonarQube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube') {
    sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mostrans-php'
              }
            }
          }
        }
      }
