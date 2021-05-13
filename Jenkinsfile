pipeline {
   agent any
   tools {
          jdk 'JDK11'
          maven 'Maven'
   }
   stages {
          stage('Install') {
                     steps {
                          sh "mvn clean install"
                     }           post {
                                    always {
                                                       junit '**/target/*-reports/TEST-*.xml'
                                    }
                     }
          }
   }
}