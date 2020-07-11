pipeline {
			agent any
			stages{
			stage('Checkout SCM') {
			steps
			{
			checkout scm
			
			}
			}
			stage ('Build'){
			steps{
			echo "Hello from build stage"
			sh "mvn clean package"
			}
			}
			stage('Test'){
			steps{
			echo "Hello from Testing stage"
			sh "mvn test"
			}
			}
			stage('Deploy'){
			steps{
			echo "Hello from Deploy stage"
}
}
}
}
