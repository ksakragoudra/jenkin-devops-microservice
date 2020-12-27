//SCRIPTED

//DECLARATIVE

pipeline {
	agent any
	stages {
		stage('Build'){
			steps{
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
			echo 'I run always...!'	
		}
		success {
			echo 'I run only when the build is success'
		}
		failure {
			echo 'I run if the build fails'	
		}
	}
}