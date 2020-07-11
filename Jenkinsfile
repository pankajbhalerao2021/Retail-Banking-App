
/* Checkout code stage */


node ('any') {
  stage('Checkout Stage') {
    checkout scm;
  }
  
  
  /* Build the source code and Perform the Unit Tests*/
  
  stage('Build and Uni Test') {
   sh 'mvn clean install'
  }
}