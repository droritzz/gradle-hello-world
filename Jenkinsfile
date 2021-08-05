#!groovy
node('slave1') {
   // Mark the code checkout 'stage'....
   stage ('Checkout'){

      // Get some code from a GitHub repository
      checkout scm
      
   }

   // Mark the code build 'stage'....
   stage ('Build'){
      // Get the gradle tool.
      def gdlHome = tool 'grandle4'
      // Run the gradle build
      sh "${gdlHome}/bin/gradle clean install"
   }
}
