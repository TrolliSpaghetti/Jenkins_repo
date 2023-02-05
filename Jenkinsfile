pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }
  def BRANCH_NAME = env.BRANCH_NAME ?: "master"
  stages {

    stage('Hello') {

      steps {

        echo env.BRANCH_NAME

      }

    }

  }

}
