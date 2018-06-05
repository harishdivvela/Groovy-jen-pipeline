pipeline
{
  agent any
  tools
  {
    maven 'Maven 3.3.9'
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
