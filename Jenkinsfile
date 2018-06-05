pipeline
{
  agent any
  tools
  {
    maven 'Maven_3.5.2'
  }
  stages
  {
    stage ('compile stage')
    {
      steps
      {
        # withMaven(maven :'Maven')
        {
          bat 'mvn clean compile'
        }
      }
    }
    
    stage ('testing stage')
    {
      steps
      {
        #withMaven(maven :'Maven')
        {
          bat 'mvn test'
        }
      }
    }

    stage ('install stage')
    {
      steps
      {
        #withMaven(maven :'Maven')
        {
          bat 'mvn clean install'
        }
      }
    }
  }
}
