//SCRIPTED

//DECLARATIVE

pipeline {
	agent any
	//agent { docker  { image 'maven:3.6.3'} }
	stages {
		stage('Build'){
			steps{
				//sh 'mvn --version'
				echo "Build"	
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo 'I run always...! testing polling'	
		}
		success {
			echo 'I run only when the build is success'
		}
		failure {
			echo 'I run if the build fails'	
		}
	}
}
