node {
  checkout scm
  sh './check_branch.sh'
  environment {
    HELLO_WORLD_SECOND='hello world 2'
  }
  echo ${env.HELLO_WORLD}
  echo ${env.HELLO_WORLD_SECOND}
  sh 'printenv'
}
