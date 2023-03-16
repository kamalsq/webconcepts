@Library('My-Jenkins-SharedLibrary') _

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
	     stage('testing'){
		    steps{
			    script{
			    	test()
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
    }
}
