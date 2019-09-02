properties([parameters([string(defaultValue: "", description: "Git Rository URL", name: 'gitRepoURL')])])
library 'JSL'

node {
   def mvnHome
   stage('Checkout app code') {
    Run.test('unit','JUNK')
    Run.test('unit', parallel = 'no')
   }
/*
stage('Checkout app code') {
      mvnTest()
   }
   stage('Code Quality') {
      sonar()
   }
   stage('Code Quality - Gates checking') {
            properties( [
          parameters([
               string(name:'stringthing', defaultValue:'mary had a little lamb', description:'string')
             ])
         ] )

      def _stringvalue = params.stringthing

      //sonarGates()
      quality-gates-jenkins(_stringvalue)
   }
   
   stage('Packaging artifacts') {
      mvnPackage()
   }
*/
}   
