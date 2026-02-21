pipeline
{
  agent any
  stages{
    stage('clone'){
      steps{
        git branch:'main',url:'https://github.com/Meharsai26/Calculator.git'
      }
    }
     stage('compile')
    {steps{
            sh 'javac Calculator.java'
          }
        }
    stage('test')
    {
      steps{
        sh 'java Calculator 30 -5'
      }
    }
    stage('Deploy')
    {
      echo 'deployment completed'
    }
   
  }
}
