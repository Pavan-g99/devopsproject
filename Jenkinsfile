pipeline{
    agent any
          options {
  buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '6')
            
  skipDefaultCheckout true


}
    stages{
        stage('checkout') {
           steps{
               checkout scm
           }
        }
       stage('hii') {
           steps{
               echo "$BUILD_NUMBER"
               print "hi hejkj"
           }
       }
         stage ('show'){
           steps{
               retry(5){
           sh 'cat cal.java'
               }
               }
           } 
       }
}
