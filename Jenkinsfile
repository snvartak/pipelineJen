pipeline{

agent any

stages{
stage('stage 1'){
steps{
withMaven(maven: 'maven_3_5_0')
  {
    sh 'mvn clean compile'
  }
}
}
stage('stage 2')
{
steps{
withMaven(maven: 'maven_3_5_0')
  {
    sh 'mvn test'
   }
}
}

stage('stage 3')
  {
    steps{
      withMaven(maven: 'maven_3_5_0)
      {
        sh 'mvn deploy'
      }
    }
  }
}
