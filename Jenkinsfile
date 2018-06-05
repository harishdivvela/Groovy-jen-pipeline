pipeline
{
  agent any
  stages
  {
    stage ('compile stage')
    {
      steps
      {
        withMaven(maven :'Maven')
        {
          sh 'mvn clean compile'
        }
      }
    }
    
    stage ('testing stage')
    {
      steps
      {
        withMaven(maven :'Maven')
        {
          sh 'mvn test'
        }
      }
    }

    stage ('install stage')
    {
      steps
      {
        withMaven(maven :'Maven')
        {
          sh 'mvn clean install'
        }
      }
    }
  }
}
