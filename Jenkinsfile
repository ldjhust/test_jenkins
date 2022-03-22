pipeline {
  agent any
  
  stages {
    stage("build") {
      steps {
        sh "echo Hello build"
      }
    }
    
    stage("test") {
      when {
        expression {
          env.BRANCH_NAME == 'master'
        }
      }
      steps {
        sh "echo Hello Test"
      }
    }
    
    stage("deploy") {
      steps {
        sh "echo hello deploy"
      }
    }
  }
}
