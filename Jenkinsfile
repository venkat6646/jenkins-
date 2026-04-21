pipeline{
	agent any
	stages{
		stage('compile')
		{
			steps{
				sh 'javac Hello.java'
			}
				
		}
		stage('run')
		{
			steps{
				sh 'java Hello'
			}
		}
	}
	post{
		always{
			echo "Pipeline completed"
		}
		success{
			echo " Successfully built"
		}
		failure{
			echo " Error occurred"
		}

	}
}
