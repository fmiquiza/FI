pipeline {
   agent any

   stages {
       stage('Build') {
           steps {
               echo 'Building..'
               sh './webappdemo/gradlew assembly'
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
