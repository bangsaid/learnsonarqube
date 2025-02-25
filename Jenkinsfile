pipeline {
        agent none
        stages {
         
          stage("build & SonarQube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
