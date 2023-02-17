pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS339 PES2UG20CS339.cpp'
    }
  }

  stage('Test') {
    steps{
      sh './PES2UG20CS339'
    }
  }

 // stage('Deploy') {
   // steps{
     // echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
