@Library('Jenkins-shared-library') _

pipeline{
	agent any
    stages{
	    stage('Code Scanning'){
		    steps{
			    script{
			    	scan()
			    }
		    }
	    }
        stage('Build'){
		    steps{
		    	script{
			    	build()
		    }
            }
        }

        stage('Deploy'){
            steps{
		       script{
			    	deploy()
		    }
            }

        }
        stage('Say thanks message'){
            steps{
		       script{
			    	saythanks()
		   	 }
        }

        }
    }
}
