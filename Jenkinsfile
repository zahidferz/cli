pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        sh 'echo "Hello from Dev"'
      }
    }

    stage('test') {
      environment {
        var = 'VARIABLE'
      }
      steps {
        sh '''echo "hello from $var" >> hello.txt
ls
echo "--------"
cat hello.txt'''
        sleep 15
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