pipeline {
  agent {
    docker {
      image 'alpine:edge'
    }

  }
  stages {
    stage('') {
      steps {
        sh '''apk add --no-cache bash curl jq gcc git go musl-dev
go mod download
bash build.sh release docker'''
      }
    }

  }
}