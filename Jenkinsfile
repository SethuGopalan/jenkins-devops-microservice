// node {
// 	echo 'Build' 
	
// 	echo "Test"

// 	echo 'Integration Test'
	
// 	}
// DECLARATIVE PIPELINE

pipeline{

	// agent any
	agent{docker{image 'python:3.8'}}
	stages{

	    stage('Build'){

		   steps{
			  sh 'python --version'
			  echo "Build"
			
		    }
	    }
	    stage('Test'){

		   steps{
			
			  echo  "Test"
			
		  }
	   }
	     stage('Integration Test'){

		     steps{
			
			    echo  "Integration Test"
		    }
	    }
	}

	post{

		always{
			echo "I am awesome. I run always"

		}
		success{
			echo "I run when you are succesfull"
			
		}
		failure{
			echo "I run when you are fail"
			
		}
 } 
}








