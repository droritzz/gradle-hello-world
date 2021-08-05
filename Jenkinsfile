#!groovy
node('slave1') {
   // Mark the code checkout 'stage'....
   stage ('Checkout'){

      // Get some code from a GitHub repository
      checkout scm
      
   }

   // Mark the code build 'stage'....
   stage ('Build'){
      sh "${gradle4}/bin/gradle build"
   }
}
