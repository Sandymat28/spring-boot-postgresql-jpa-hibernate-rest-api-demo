pipeline {

  agent any

  tools {
    maven 'maven:3.9.9'
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
      }
    }
    
    stage("deploy"){
      
      steps{
          echo 'deploying application'
      }
    }
    
  }
  
}
