pipeline {
   agent any
  
   stages {
        stage('One') {
                 steps {
                     input('this is nilesh devops engineer .will you like to start devlopmen')
                 }
                 }
        stage('two') {
            parallel{
                stage('p1') {
                 steps { echo'parllel stage 1'}
                      }
                stage('p2') {
                 steps { echo'parllel stage 2'}
                      }
                    }    
        }
        stage('Build') {
               agent   {docker {image 'ubuntu'}
         }
         steps {
           
            sh "uname -a"

               }
         
        }
       
}
}
