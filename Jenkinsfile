node('maven-jdk-8') {
  stage 'Build and Verify'
  checkout scm
  sh('git rev-parse HEAD > GIT_COMMIT')
  git_commit=readFile('GIT_COMMIT')
  short_commit=git_commit.take(7)
  echo "$short_commit"
  sh 'mvn verify'
  }
Contact GitHub API Training Shop Blog About
