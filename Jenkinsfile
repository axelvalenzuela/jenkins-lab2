pipeline{
	agent{label 'master'}
	stages{
		stage('Checkout'){
			steps{
				git branch: 'master', url: 'https://github.com/axelvalenzuela/jenkins-lab2.git'
			    }
		}
    	stage('Setup'){
      			steps{
				sh 'chmod +x install.sh'
        			sh './install.sh'
      			}
    	}
    	stage('Test'){
      			steps{
				 sh '''#!/bin/bash
				     source myprojectenv/bin/activate
                		     python -m unittest
				     '''
            	}
   		}
	}
}
