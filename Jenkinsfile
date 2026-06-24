pipeline {
  agent any 
  stages {
    stage ('build'){
      steps {
         echo " the pipeline is ${env.BRANCH_NAME} "
         }
       }
     stage ('UAT') {
       when {
         branch 'UAT'
       }
       steps{
         echo "Deploy this to UAT"
       }
     }
     stage ('Dev') {
       when {
         branch 'Dev'
       }
       steps{
         echo "Deploy this to Dev"
       }
     }
     stage ('Prod') {
       when {
         branch 'Prod'
       }
       steps{
         echo "Deploy this to Prod"
       }
     }
     stage ('main') {
       when {
         branch 'main'
       }
       steps{
         echo "Deploy this to main"
       }
     }
  }
}
