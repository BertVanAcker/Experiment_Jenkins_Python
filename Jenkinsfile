pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        sh 'python --version'
      }
    }
	stage('install dependencies') {
        steps {
            sh 'python -m pip install -r requirements.txt'
        }
	}
    stage('hello') {
      steps {
        sh 'python src/hello.py'
      }
    }
  }
}