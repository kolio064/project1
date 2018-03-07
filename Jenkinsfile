pipeline {
    environment {
	work_dir = "/home/www/staging"
    }
    agent any
    stages {


    stage('Example') {
        if (env.BRANCH_NAME == 'master') {
            echo 'I only execute on the master branch'
        } else {
            echo 'I execute elsewhere'
        }
    }



        stage('Build') {
            steps {
		sh 'printenv'
	        echo '======>>> this is env.GIT_BRANCH...' + env.GIT_BRANCH
                echo 'Hello World One'
		echo 'Hello World Two'
		echo 'Hello World Three'}
	}
	stage('Testing1') {
	    steps {
		sh 'php -v' }
        }
	stage('Testing2') {
	    steps {
		sh 'date' }
	}
	stage('Testing3') {
	    steps {
		sh 'cd /home/staging/ && pwd && ls -lha'
		sh 'pwd'
		}
	}
	stage('Testing4') {
	    steps {
		sh '''
		echo "Testing Multiline Shell Steps"
		cd /home/staging/
		pwd
		'''
		}
	}
    }
}