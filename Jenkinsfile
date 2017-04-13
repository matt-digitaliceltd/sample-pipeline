node {
  checkout scm

  buildType = sh(script: './check_branch.sh', returnStdout: true)

  environment {
    HELLO_WORLD_SECOND='hello world 2'
  }
  echo "$buildType"
  sh 'printenv'
}
