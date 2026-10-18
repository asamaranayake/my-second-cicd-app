pipeline {
  agent any 

  tools{
    nodejs 'Node 24'
  }

  stages{
    stage('Checkout'){
      steps{
        git 'https://github.com/asamaranayake/my-second-cicd-app.git'
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
  
