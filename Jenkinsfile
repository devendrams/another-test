pipeline {
  agent any
  
  stages {
    stage('Unit test') {
      steps {
        sh 'ant -f test.xml -v'
        junit 'reports/result.xml'
      }
    }
    stage('build') {
	steps {
	      sh 'ant -f build.xml -v'
       }
    }
  }
}
