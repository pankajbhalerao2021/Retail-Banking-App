/* This is reusable jenkinsfile for maven project.

Contributors:
Version:1.0.0

This snippet will:
	
	-Run the source code using maven,
	-Run the code quality using sonar,
	-Run unit test if any,
	-Push the generated artifacts in to Nexus repository
	
*/


	
	Properties([
	
	[$class : 'BuildDiscarderProperty', strategy : [ $class : 'LogRotator', daysToKeepStr: '1', numToKeepStr: '5']],
	pipelineTriggers([githubpush()]),
	parameters([
	
	choice(choices: 'Snapshot\nRelease',description: 'Do you need snapshot or release?', name: 'Requested_Action' )
	])
	])
	
	
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
	