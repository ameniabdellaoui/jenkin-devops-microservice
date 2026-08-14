//SCRIPTED
//DECLARATIVE
pipeline {
	// agent any
	// agent { docker { image 'maven:3.6.3'}}
	agent{ docker{image 'node:26.7.0'}}
	stages{
		stage('Build'){
			steps{
				sh "node --version"
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
	post{
			always{
				echo "I am awesome, I run always"
			}
			success{
				echo "I run when success!"
			}
			failure{
				echo "I run when it is a failure"
			}
		}
}
