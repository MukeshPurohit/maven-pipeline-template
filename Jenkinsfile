library 'JSL'

properties([parameters([string(defaultValue: "refs/heads/master", description: "Git Rository URL", name: 'GitCheckout')])])


node {
	dryrun{
		repo = 'test1'
		folder = 'test2'
		submodules = true
		refs = params.GitCheckout
	}
println "******************"	
println params.GitCheckout
println "******************"
/*
node {
   def mvnHome
   stage('Checkout app code') {
    //dryrun.test('unit','junk')
    //dryrun.test('unit', parallel = 'no')
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

      //sonarGates()
      quality-gates-jenkins(_stringvalue)
   }
   
   stage('Packaging artifacts') {
      mvnPackage()
   }
*/
}   
