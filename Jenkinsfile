pipeline{
	agent any

	stages{
	    stage('Checkout'){
	       steps{
              git 'https://github.com/harshamullapudi/JenkinsProject.git'
	      }
	    }

		stage('Build'){
			steps{
				echo 'Building the application'
			}
		}

		stage('Test'){
			steps{
				sh 'python3 $WORKSPACE/myfile.py'
				//sh 'ls -a'
				echo 'Script is working fine'
			}
		}

		stage('Deploy'){
			steps{
				echo 'Deploying the application'
			}
		}
    }
    post{
    	always{
    		echo 'Pipeline finished'
    	}
    }

}