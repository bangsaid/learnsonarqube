pipeline {
        agent none
        stages {
         
          stage("build & SonarQube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube Server') {
    sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mostrans-php'
              }
            }
          }
        }
      }
