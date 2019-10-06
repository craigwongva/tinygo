node {
    stage('welcomex') {
      sh 'echo welcomey'
    }

    stage('rebuildApp') {
      git(
        url: 'https://github.com/craigwongva/tinygo.git',
        branch: "master"
      )

      sh """
pwd # /var/lib/jenkins/workspace/src/tinygo
export GOPATH=/var/lib/jenkins/workspace/src/tinygo
go get ./pkg/main
"""
      //sh 'export GOPATH=/var/lib/jenkins/workspace/src/tinygo'
      //sh 'go run main.go'
    }
}
