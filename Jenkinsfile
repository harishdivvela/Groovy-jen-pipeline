pipeline
{
  agent any
  stages
  {
    stage ('compile stage')
    {
      steps
      { 
        withMaven(maven : 'maven_3.3.9')
      {
          bat 'mvn clean compile'
        }
      }
    }
    stage ('testing stage')
    {
      steps
      {
        withMaven(maven : 'maven_3.3.9')
      } 
        {
          bat 'mvn test'
        }
    }

    stage ('install stage')
    {
      steps
      {
        withMaven(maven : 'maven_3.3.9')
      }        
        {
          bat 'mvn clean install'
        }
      }
  }
}
