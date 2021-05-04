pipeline{
agent {
label 'kishore'
}

stages {

stage ('Checkout')
{
steps
     {
      
          checkout scm

     }

}
stage ('Build1')
{
   steps
   {
     echo "Building has been started"
   }
}
   stage('Test')
{
   steps
   { 
     echo "Testing has been started"
   }
}
   stage ('Deployment')
{
steps{
    node ('K8S-MASTER')
    {
      echo "Deployment has been started"
    }
}

}

}

}

