work_dir = '/home/staging/www'

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
		echo 'Hello World'
		echo 'Hello World Times Three'}
}
	stage('Testing1') {
	    steps {
		sh 'php -v' }
        }
	stage('Testing2') {
	    steps {
		sh 'pwd' }
	}
	stage('Testing3') {
	    steps {
		sh 'cd /home/staging/ && pwd'
		}
	}
	stage('Testing4') {
	    steps {
		sh 'ls -lha' }
	}
    }
}