pipeline {
    agent any

stages{
    stage('git-clone-build') {
      steps {
        parallel(
          a: {
            echo "git clone"
          },
          b: {
            echo "build"
          }
        )
      }
    }
      
      stage('test'){
          steps{
              echo "test - git jenkins"
          }
      }
      
      stage('deploy'){
          steps{
              echo "deploy - git jenkins"
          }
      }
    }
}
