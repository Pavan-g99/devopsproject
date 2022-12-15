pipeline{
    agent{ 
        label 'linux'
          }
          options {
  buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '6')
}
    stages{
       stage('hii') {
           steps{
               echo "$BUILD_NUMBER"
               print "hi hejkj"
           }
       }
         stage ('show'){
           steps{
           sh 'cat cal.java'
               }
           } 
       }
}
