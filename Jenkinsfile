pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        sh 'go build -v -o simple-cal -ldflags "-s -w"'
        sh 'go test -v'
        archiveArtifacts 'simple-cal'
      }
    }

  }
}