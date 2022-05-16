pipeline {
  agent any
  tools { 
        maven 'Maven 3.8.5'
        jdk 'jdk17'
        git 'git'
    
    }
  stages {
    stage('Git') {
      steps {
        echo 'Hej Arbetswplats!'
        echo env.WORKSPACE
      }
    }

  }
}