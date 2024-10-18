pipeline {

  agent any

  tools {
    Maven 'maven:3.9.9'
  }
  
  stages {
    
    stage("build"){
      
      steps {
          echo 'building application'
          sh 'maven clean install'
      }
    }
    
    stage("test"){
      steps {
          echo 'testing application'
          sh 'mvn test'
      }
    }

    stage("package"){
       steps {
          echo 'packaging application'
          sh 'mvn package'
       }
      
    stage("deploy"){
      
      steps{
          echo 'deploying application'
          sh 'mvn deploy'
      }
    }
    
  }
  
}
