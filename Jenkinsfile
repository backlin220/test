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
        echo 'Hej Arbetsplats 2!'
        echo env.WORKSPACE
      }
    }
    stage('Maven') {
      steps {
        bat 'mvn clean verify sonar:sonar \\   -Dsonar.projectKey=mvn-basic \\  -Dsonar.host.url=http://localhost:9000 \\  -Dsonar.login=63ec183205d770759baf33b18d0a4312ab94b5a8'
      }
    }

  }
}