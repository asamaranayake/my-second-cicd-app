pipeline {
  agent any 

  tools{
    nodejs 'Node 24'
  }

  stages{
    stage('Checkout'){
      steps{
        checkout scm
      }
    }
    stage('Install'){
      steps{
        sh 'npm install'
      }
    }
    stage('Test'){
      steps{
        sh 'npm test'
      }
    }
    stage('Run'){
      steps{
        sh 'npm start'
      }
    }
  }
}
  
