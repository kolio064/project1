pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'}
	    steps {
		echo 'Hello World'}
	    steps {
		echo 'Running Setup Stage'}
	stage('Setup') {
    		sh 'su - jenkins -c "php -v"'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

