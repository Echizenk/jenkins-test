pipeline {
    agent any
	options {
	buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
	disableConcurrentBuilds()
}
    stages {
        stage('Build') {
            steps {
		echo "Hello"
            }
        }
	stage('cat README'){
	when {
		branch "fix-*"
	}
	steps {
	sh '''
		cat README.md
	'''
	}
	}
    }
}
