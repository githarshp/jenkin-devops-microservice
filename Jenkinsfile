// Declarative Pipeline
pipeline {
	agent { docker { image 'maven:3.6.3' } }
	stages {
		stage ('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage ('Test') {
			steps {
				echo "Test"
			}
		}
		stage ('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
		post {
			always{
				echo 'I always run'
			}
			success{
				echo 'I run upon success'
			}
			failure{
				echo 'I run upon failure'
			}
	  }
}