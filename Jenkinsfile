pipeline {
  agent any
  stages {
    stage('set env') {
      steps {
        sh '''export PATH=$PATH:/usr/local/go/bin
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
export GO111MODULE=auto'''
      }
    }

    stage('check version') {
      steps {
        sh 'echo $PATH'
        sh 'go version'
        sh 'go build'
      }
    }

  }
}