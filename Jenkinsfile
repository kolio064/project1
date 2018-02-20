pipeline {
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
	stage('Testing2')
	dir ('/home/www/staging'){
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