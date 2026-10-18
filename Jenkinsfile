pipeline{
  agent any 

  tools{
    nodejs 'Node 24'
  }

  stages{
    stage('Checkout'){
      step{
        git 'https://github.com/asamaranayake/my-second-cicd-app.git'
      }
    }
    stage('Install'){
      step{
        sh 'npm install'
      }
    }
    stage('Test'){
      step{
        sh 'npm test'
      }
    }
    stage('Run'){
      step{
        sh 'npm start'
      }
    }
    

  }

  
