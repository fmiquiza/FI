pipeline {
   agent any

   stages {
       stage('Build') {
           steps {
               echo 'Building..'
               sh './webappdemo/gradlew assemble'
               archiveArtifacts 'webappdemo/build/reports/test/*.war'
           }
       }
       stage('Test') {
           steps {
               echo 'Testing..'
               sh './webappdemo/gradlew test'
           }
       }
       stage('Deploy') {
           steps {
               echo 'Deploying......'
           }
       }
   }
}
