pipeline {
  agent any
  stages {
    stage('Start Work') {
      steps {
        echo 'Begin'
        sh '''ls
pwd
echo $GOPATH
echo "${GOROOT}"'''
        sh '''go version
ssh 
scp
'''
      }
    }

  }
}