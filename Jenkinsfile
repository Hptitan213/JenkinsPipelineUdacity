pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        sh 'echo "Hello World"'
        sh '''
            echo "Multiline shell steps works too"
            ls -lah
        '''
      }
    }
    stage('Lint HTML') {
      steps {
        sh 'tidy -q -e *.html'
      }
    }
    stage('AWS Upload') {
      steps {
        sh 's3Upload(file:\'index.html\', bucket:\'udacityfour\', path:\'index.html\')'
      }
    }
  }
}