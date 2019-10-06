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
go get ./pkg/main
/var/lib/jenkins/workspace/bin/main
cd /var/lib/jenkins/workspace/src/tinygo
ls
../../golint ./...
echo I just finished golint
"""
 }
}
