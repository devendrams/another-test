pipeline {
  agent any

  stages {
    stage('build') {
        steps {
              sh 'ant -f build.xml -v'
       }
    }
  }
  
  always {
    archive 'dist/*.jar'
  }
}
