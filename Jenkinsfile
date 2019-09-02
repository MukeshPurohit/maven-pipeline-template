library 'JSL'

properties([parameters([string(defaultValue: 'refs/heads/master', description: 'Git Rository URL', name: 'GitCheckout')])])

//def myInput = input message: 'Enter parameters', parameters: [string(defaultValue: '', description: '', name: 'DEMO1'), string(defaultValue: '', description: '', name: 'DEMO2'), string(defaultValue: '', description: '', name: 'DEMO3')]

def refs = params.GitCheckout
node {
	dryrun{
		repo = 'test1'
		folder = 'test2'
		submodules = true
		refs = refs
	}

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
