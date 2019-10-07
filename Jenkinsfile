node {

    stage('rebuildApp') {
      environment {
        GOPATH = "frogs"
      }
    
      git(
        url: 'https://github.com/craigwongva/tinygo.git',
        branch: "master"
      )
      
      sh """
pwd # /var/lib/jenkins/workspace/src/tinygo
echo $GOPATH
go install ./pkg/tinygok
"""
 }
}
