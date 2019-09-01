library 'JSL'

node {
   def mvnHome
   stage('Checkout app code') {
      fetchCode()
   }
   stage('Checkout app code') {
      mvnTest()
   }
   stage('Code Quality') {
      sonar()
   }
   stage('Packaging artifacts') {
      mvnPackage()
   }
   
   stage('Display Results') {
      mvnResultsSureFire()
   }
}
   
/*
stage('Build') {
      withEnv(["MVN_HOME=$mvnHome"]) {
         if (isUnix()) {
            sh '"$MVN_HOME/bin/mvn" -Dmaven.test.failure.ignore clean package'
         } else {
            bat(/"%MVN_HOME%\bin\mvn" -Dmaven.test.failure.ignore clean package/)
         }
      }
   }
*/
   
