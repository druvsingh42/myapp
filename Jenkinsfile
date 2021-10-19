node{

  stage('SCM Checkout')
  {
    
     def mvnHome = tool name: 'maven3', type: 'maven' 
     echo "in the checkout"
    sh "{mvnHome}/bin/mvn clean" 
    
  }
  
    stage('Install Package')
  {
    echo 'in the install'
    sh "{mvnHome}/bin/mvn install" 
  }


}
