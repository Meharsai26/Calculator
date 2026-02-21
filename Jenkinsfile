pipeline
{
  agent any
  stages{
    stage('clone'){
      steps{
        git branch:'main',url:''
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
      steps
      {
        echo 'Deployment completed'
      }
    }
    stage('build')
    {
      steps{
        sh 'java Calculator 25 5'
      }
    }
  }
}
