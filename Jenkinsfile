pipeline{
	agent any

	stages{
	    stage('Checkout'){
	       steps{
              git clone https://github.com/harshamullapudi/JenkinsProject.git
	      }
	    }
	}

	stage('Build'){
		steps{
			echo 'Building the application'
		}
	}

	stage('Test'){
		steps{
			sh 'python3 myfile.py'
		}
	}

	stage('Deploy'){
		steps{
			echo 'Deploying the application'
		}
	}
    
    post{
    	always{
    		echo 'Pipeline finished'
    	}
    }

}