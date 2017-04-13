node {
  checkout scm

  buildType = sh(script: 'check_branch.sh', returnStdout: true)

  environment {
    HELLO_WORLD_SECOND='hello world 2'
  }
  echo ${buildType}
  echo ${env.HELLO_WORLD}
  echo ${env.HELLO_WORLD_SECOND}
  sh 'printenv'
}
