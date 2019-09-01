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
            properties( [
          parameters([
               string(name:'stringthing', defaultValue:'mary had a little lamb', description:'string')
             ])
         ] )

      def _stringvalue = params.stringthing

      paramEcho {
          stringvalue = _stringvalue
      }
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
