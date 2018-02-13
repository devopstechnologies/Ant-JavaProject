stage 'Init'
node {
  checkout scm
  'echo $BRANCH_NAME'
  bat 'ant'
}
if (env.BRANCH_NAME == 'master') {
  stage 'Only on master'
  println 'This happens only on master'
} else {
  stage 'Other branches'
  println "Current branch ${env.BRANCH_NAME}"
}

