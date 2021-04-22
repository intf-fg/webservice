pipeline {
  agent any
  stages {
    stage('Pull_FT') {
      agent {
        node {
          label 'FT'
        }

      }
      steps {
        sh 'docker build /home/FT/Jenkins/workspace/1_Pull_FT -t webservice'
        sh 'docker run -it -p 82:80 -d webservice'
      }
    }

  }
}