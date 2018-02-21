pipeline {
environment {
work_dir = "/home/www/staging"
}
    agent any

    stages {
        stage('Build') {
            steps {
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
		sh 'ls -lha' }
	}
    }
}