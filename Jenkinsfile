pipeline {
	agent any
	stages {
		stage('checkout') {
			steps {
				checkout scm
			}
		}
		stage('shellcheck') {
			steps {
				sh 'find . -name "*.sh" |xargs shellcheck'
			}
		}
	}
}
