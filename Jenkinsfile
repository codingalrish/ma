pipeline {
   agent any

   stages {

       stage('Build') {
           steps {
               Echo 'hello'
           }
       }
   }

   post {

       success {
           mail to: 'student@gmail.com',
           subject: 'Build Success',
           body: 'Maven build completed and artifact created successfully.'
       }

       failure {
           mail to: 'student@gmail.com',
           subject: 'Build Failed',
           body: 'Please check Jenkins logs.'
       }
   }
}
