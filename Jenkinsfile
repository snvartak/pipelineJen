pipeline{

agent any

stages{
stage('stage 1'){
steps{
withMaven  {
    sh 'mvn clean compile'
  }
}
}
stage('stage 2')
{
steps{
withMaven
  {
    sh 'mvn test'
   }
}
}

stage('stage 3')
  {
    steps{
      withMaven
      {
        sh 'mvn deploy'
      }
    }
  }
}
}
