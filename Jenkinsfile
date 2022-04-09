pipeline {
	agent any 
	
	stages {
		stage('Build') {
			steps{
				echo 'Building...'
				sh """
				docker build -t python_app1 .
				"""
			}
		}
                stage('Test') {
                        steps{
                                echo 'Testing...'
				sh """
				docker run --rm --name py_app1 python_app1
				"""
                        }
                }
                stage('Deploy') {
                        steps{
                                echo 'Deploying...'
				
                        }
                }

	}

}
