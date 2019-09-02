library 'JSL'

properties([parameters([string(defaultValue: 'https://github.com/jglick/simple-maven-project-with-tests.git', description: 'Enter Git Rository URL', name: 'GitURL'),
string(defaultValue: 'refs/heads/master', description: 'Checkout Type', name: 'GitCheckoutType')])])

//def myInput = input message: 'Enter parameters', parameters: [string(defaultValue: '', description: '', name: 'DEMO1'), string(defaultValue: '', description: '', name: 'DEMO2'), string(defaultValue: '', description: '', name: 'DEMO3')]

def gitRepo = params.GitURL
def refs = params.GitCheckoutType
node {
	dryrun{
		repo = gitRepo
		references = refs
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
