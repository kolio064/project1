pipeline {
    environment {
	WORK_DIR = "/home/www/staging"
	WE_BUILD_ONLY_ON="master"
    }

    agent any

    stages {

        stage('Build') {
	    when {
		expression { BRANCH_NAME == WE_BUILD_ONLY_ON }
	    }
            steps {
		echo 'We are in Build .... CONTINUE ... we are in master !!!'


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