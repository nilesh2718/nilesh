pipeline {

   agent any
  
   stages {

    stage("Env Variables") {
            steps {
              echo 'Testing environment veriables'

                sh 'echo"$BUILD_NUMBER"'
            }
        }
    stage('Input step') {
                 steps {

                  echo'Testing human input authorization (input)'
                  input('this is nilesh devops engineer .will you like to start devlopmen')
                 }
                 }
    stage('two') {

            parallel{

                stage('p1') {
                 steps { echo'Running two steps at same time P1'}
                      }
                stage('p2') {
                 steps { echo'Running two steps at same time P2'}
                      }
                    }    
        }
    stage('Build') {
              
         
         steps {
           
            sh "uname -a"

               }
         
        }
       
}
}
