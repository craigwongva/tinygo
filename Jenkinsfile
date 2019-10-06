node {
    stage('welcomex') {
      sh 'echo welcomey'
    }

    stage('rebuildApp') {
      git(
        url: 'https://github.com/craigwongva/tinygo.git',
        branch: "master"
      )

      withEnv([GOPATH="/var/lib/jenkins/workspace/src/tinygo"]) {
//            sh 'go version'
/*
      sh """
pwd # /var/lib/jenkins/workspace/src/tinygo
echo $GOPATH
go build ./pkg/main
"""
*/
     }
      //sh 'export GOPATH=/var/lib/jenkins/workspace/src/tinygo'
      //sh 'go run main.go'
    }
}
