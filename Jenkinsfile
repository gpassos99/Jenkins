pipeline {
   agent any
   tools {
          jdk 'JDK11'
          maven 'Maven'
   }
   stages {
          stage('test java installation') {
                     steps {
                                    sh 'java -version'
                     }
          }
          stage('test maven installation') {
                     steps {
                                    sh 'mvn -version'
                     }
          }
   }
}