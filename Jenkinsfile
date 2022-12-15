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
        post{
           success{
               echo "jub success at stage leval"
           } 
           failure{
               print "job failed at stage level"
           }
       }
         stage ('show'){
           steps{
           sh 'cat cal.java'
           }
         }
    
       }
    }
    post {
        success{
            echo "job success at global level"
        }
        failure{
            echo "job failed at global level"
        }
        cleanup{
            echo "cleaning up at global level"
        }
    }
}
