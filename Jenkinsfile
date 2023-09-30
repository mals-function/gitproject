pipeline {
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Malou Aday'
			
                }
        }
	    stage('Two'){
		    
		steps {
			input('Do you want to proceed?')
        }
	    }
        stage('Three') {
                when {
                        not {
                                branch "master"
                        }
                }
                steps {
			echo "Hello Again. :)"
                        }
        }
        stage('Four') {
                parallel {
                        stage('Unit Test') {
                                steps{
                                        echo "Running the unit test..."
                                }
                        }
                       
                               
			}  }
        }
    }


