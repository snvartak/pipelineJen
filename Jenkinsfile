pipeline{

agent any

stages{

withMaven  {
    sh 'mvn clean compile'
  }
}
stage('stage 2')
{
withMaven
  {
    sh 'mvn test'
   }
}

stage('stage 3')
  {
      withMaven
      {
        sh 'mvn deploy'
      }
    }
}
