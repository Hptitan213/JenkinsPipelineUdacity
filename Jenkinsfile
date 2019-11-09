pipeline {
  agent any
  stages {
    stage('Hello World') {
      steps {
        sh 'echo "Hello World"'
        sh '''
            echo "Multiline shell steps works too"
            ls -lah
        '''
      }
    }

  }
}