pipeline
{
  agent any
  stages
  {
    stage ('compile stage')
    {
      steps
      {
        withMaven(maven :'Maven 3.3.9')
        {
          sh 'mvn clean compile'
        }
      }
    }
    
    stage ('testing stage')
    {
      steps
      {
        withMaven(maven :'Maven 3.3.9')
        {
          sh 'mvn test'
        }
      }
    }

    stage ('install stage')
    {
      steps
      {
        withMaven(maven :'Maven 3.3.9')
        {
          sh 'mvn clean install'
        }
      }
    }
  }
}
