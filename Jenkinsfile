pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/Devops-trainer1987/ctsproj1.git'
         }
      }
     /* stage('Compile') {
         steps {
            bat 'mvn compile'
         }
      }
	   stage('Test') {
         steps {
            bat 'mvn test'
         }
      }*/
	   stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/Windows/System32/config/systemprofile/AppData/Local/Jenkins/.jenkins/workspace/cts_pipeline/target/ctsproj1-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
