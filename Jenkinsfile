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
          bat 'mvn clean compile'
        }
      }
    
    stage ('testing stage')
    {
      steps
      
        
        {
          bat 'mvn test'
        }
      
    }

    stage ('install stage')
    {
      steps        
        {
          bat 'mvn clean install'
        }
      }
   
  }
}
