pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        sh 'echo "Hello from Dev"'
      }
    }

    stage('test') {
      steps {
        sh '''echo "hello from test" >> hello.txt
ls
echo "--------"
cat hello.txt'''
      }
    }

    stage('final') {
      steps {
        sh '''cat hello.txt
ls
echo "------------final----"'''
      }
    }

  }
}