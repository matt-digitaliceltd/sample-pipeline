def buildType = ''
script {
  println env.branch
  buildType = 'RC'
}
node {
  checkout scm

  //buildType = sh(script: './check_branch.sh', returnStdout: true)

  echo "$buildType"
  sh 'printenv'
}
