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
   stage('Code Quality - Gates checking') {
      //sonarGates()
      quality-gates-jenkins()
   }
   
   stage('Packaging artifacts') {
      mvnPackage()
   }
   /*
   stage('Display Results') {
      mvnResultsSureFire()
   }
   */
}   
