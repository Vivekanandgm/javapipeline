pipeline {
  agent any
  stages {
    stage ('Git-checkout') {
      steps {
      git branch: 'main', credentialsId: '60f4c8a4-374f-48b1-87cf-816a3c48144d', url: 'https://github.com/Vivekanandgm/javapipeline.git'
      }
    }
    stage ('Maven-Build') {
      steps {
      sh '''
        mvn clean package
        '''
      echo "Building java code using maven"
      }
    }
  }
}
