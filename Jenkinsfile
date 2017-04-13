def branchName = ''
def buildType = ''
def devStream = ''
script {
  if (BRANCH == 'OTHER') {
    branchName = BRANCH_OTHER
    buildType = 'DEV'
    devStream = 'OTHER'
  } else if (BRANCH ==~ /Releases\/.+$/) {
    branchName = BRANCH
    buildType = 'RC'
    devStream = 'Release'
  } else {
    branchName = BRANCH
    buildType = 'DEV'
    devStream = '' //need to get the base branch name
  }
}
node {
  checkout scm

  //buildType = sh(script: './check_branch.sh', returnStdout: true)

  echo "type: $buildType, name: $branchName, stream: $devStream"

}
