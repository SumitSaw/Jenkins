pipeline {
	agent any
	stages {
		stage('Compile') {
			steps {
					echo "Compliled Successfully !";
			}
		}
		
		stage('JUnit') {
			steps {
					echo "JUnit passed successfully !";
			}
		}
		
		stage ('Quality-Gate')	{
			steps {
					echo " SonarQube Quality Gate passed successfully";\
					
			}
		}
		stage('deploy') {
			steps {
					echo "Deployment passed";
			}
		}
					
	post {
		always {
				echo 'This will always run'
		}
		success {
				echo 'Thi will run only if success'
		}
		failure {
				echo 'This will run only if failed'
		}
		unstable {
				echo 'This will run only if run marked as unstable'
		}
		chnaged {
				echo 'This will only run if the state of the pipelinehas changed'
				echo 'for exmample, If the pipeline was previously failing but is now successfull'
		}
		
	}
	
}
		
	
		
		
		
		
		
		
		
		
		
		
		
		
			
		
