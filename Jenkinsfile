pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS399 PES2UG20CS399.cpp'
    }
  }

  stage('Test') {
    steps{
      sh './PES2UG20CS309'
    }
  }

 stages('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
