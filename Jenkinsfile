pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        sh 'echo "Upload to S3"'
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

  }
}