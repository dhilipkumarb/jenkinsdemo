pipeline {
	agent {
		label 'Worker'
	}
	stages {
		stage('Build') {
			steps {
				echo "Would have run the build related steps";
			}
		}
		
		stage('Test') {
			steps {
				echo "Would have run the test cases in this step";
			}
		}
		
		stage('Disable Monitoring') {
			steps {
				echo "Would have Disabled current monitoring setup";
			}
		}
		
		stage('Deploy') {
			steps {
				echo "Would have deployed the service to desired environment";
			}
		}
		
		stage('Re-enable Monitoring') {
			steps {
				echo "Would have re-enabled monitoring setup";
			}
		}
		
	}
	post {
		always {
			echo "This pipeline execution was executed, results will vary";
		}
		success {
			echo "Success status will be shared with the group";
		}
		failure {
			echo "Failure status will be shared with the group";
		}
		unstable {
			echo "Build or one of the stages have failed, and want to mark it as unstable";
		}
		changed {
			echo "Previous pipeline was failure, but this one works fine!";
		}
	}
}
