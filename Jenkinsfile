pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }
  stages {

    stage('Hello') {
      when {
          expression {
            return fileExists('README.md')
          }
        }
      steps {
        echo 'file exist!!'
      }
    }
       stage('Hello3') {
        steps {
        echo "Branch Name"
        echo env.BRANCH_NAME
        echo "Change_Target" 
        echo env.CHANGE_TARGET
        echo "Wrokspace" 
        echo env.WORKSPACE

      }

    }

  }

}
