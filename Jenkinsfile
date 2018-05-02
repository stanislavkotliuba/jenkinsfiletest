pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh '''export TEST1TEST="test1";
              export TEST2TEST="test2";
              echo $TEST1TEST;
              echo $BUILD_TIMESTAMP;
              echo $TEST2TEST'''
      }
    }
    stage('Testing') {
      steps {
        sh 'chmod +x ./hellokitty.sh'
        sh './hellokitty.sh'
      }
    }
    stage('Activate release') {
      steps {
        sh 'echo "here will be activate release -tasks"'
      }
    }
  }
}
