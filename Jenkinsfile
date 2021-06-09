pipeline {
    agent {
	label 'agent1'
	}

    stages {
        stage('Git-Checkout') {
            steps {
                echo 'Clone Repository from GitHub'
			
                git 'https://github.com/deepak83s143/git-labs.git'
            }
        }
        stage('Compile') {
            steps {
                echo 'Code is Compiling'
            }
        }
        stage('CodeReview') {
            steps {
                echo 'After Compiling now code is reviewing'
            }
        }
        stage('UnitTest') {
            steps {
                echo 'Testing of Code'
            }
        }
        stage('MetricCheck') {
            steps {
                echo 'Checking......>>>>'
            }
        }
        stage('Packaging') {
		steps {
                echo 'Create package from raw code '
                sh 'sudo cp index.html /var/www/html'
                sh 'sudo service httpd restart'
            }
        }    
    }
}
