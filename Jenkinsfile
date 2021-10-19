node{

  stage('SCM Checkout')
  {
    
     def mvnHome = tool name: 'maven3', type: 'maven' 
     git branch: 'main', url: 'https://github.com/druvsingh42/myapp.git'
     echo "in the checkout"
    sh "${mvnHome}/bin/mvn clean" 
    
  }
  
    stage('Install Package')
  {
    def mvnHome = tool name: 'maven3', type: 'maven' 
    echo 'in the install'
    sh "${mvnHome}/bin/mvn install" 
  }


}
