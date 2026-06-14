pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'python -m py_compile sources/addvals2.py sources/calc.py'
        stash(name: 'compiled-results', includes: 'sources/*.py*')
      }
    }
  }
}