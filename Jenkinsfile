pipeline {
	//agent any
	agent { docker { image 'maven:3.8.4' } }
	stages {
		stage('Build') {
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
		always {
			echo 'Im awesome, I run always'
		}
		success {
			echo 'I run when you are sucessful'
		}
		failure {
			echo 'I run when you fail'
		}
	}

}
