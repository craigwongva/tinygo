node {
    stage('welcomex') {
      sh 'echo welcomey'
    }

    withEnv([GOPATH="/var/lib/jenkins/workspace/src/tinygo"]) {
    stage('rebuildApp') {
      git(
        url: 'https://github.com/craigwongva/tinygo.git',
        branch: "master"
      )

//            sh 'go version'
/*
      sh """
pwd # /var/lib/jenkins/workspace/src/tinygo
echo $GOPATH
go build ./pkg/main
"""
*/
     }
    }
}
