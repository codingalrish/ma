pipeline {
   agent any

   stages {

       stage('Build') {
           steps {
               echo 'hello'
           }
       }
   }

   post {

       success {
           mail to: 'codingalrish@gmail.com',
           subject: 'Build Success',
           body: 'Maven build completed and artifact created successfully.'
       }

       failure {
           mail to: 'codingalrish@gmail.com',
           subject: 'Build Failed',
           body: 'Please check Jenkins logs.'
       }
   }
}
