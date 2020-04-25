pipeline {
  agent any
  stages {
    stage('Start Work') {
      steps {
        echo 'Go env config'
        sh '''export PATH=$PATH:/usr/local/go/bin
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
export GO111MODULE=auto'''
        sh 'go version'
      }
    }

  }
}