pipeline {
  agent any
  stages {
    stage('Start Work') {
      steps {
        echo 'Go env config'
        sh '''export PATH=$PATH:/usr/local/go/bin
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
export GO111MODULE=auto
'''
        sh '/usr/local/go/bin/go version'
        sleep(time: 1, unit: 'SECONDS')
        sh '/usr/local/go/bin/go env'
      }
    }

  }
}