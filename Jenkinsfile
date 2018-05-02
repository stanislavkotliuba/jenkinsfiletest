pipeline {
  agent any
  stages {
    stage('Deploy/Symlink/Composer install') {
      steps {
        sh '''export TEST1TEST="test1";
              export TEST2TEST="test2";
              echo $TEST1TEST;
              echo $TEST2TEST'''
      }
    }
    stage('Testing') {
      steps {
        sh 'echo "here will be tests"'
    }
  }
}
