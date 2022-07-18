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
          sh 'ls'
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
          sh 'ls'
        }
    }

    stage ('install stage')
    {
      steps
      {
        withMaven(maven : 'maven_3.3.9')
      }        
        {
          sh 'ls'
        }
      }
  }

}
