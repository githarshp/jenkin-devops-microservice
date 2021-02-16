// Declarative Pipeline
pipeline {
	agent any
	stages {
		stage ('Build') {
			steps {
				echo "build"
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
}