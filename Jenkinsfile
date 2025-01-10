pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        echo "Github checkout"
      }
    }

    stage('Build'){
      steps{
        echo "Building project"
      }
    }

    stage('Test'){
      steps{
        echo "Testing project"
      }
    }

    stage('Staging'){
      steps{
        echo "Copying artifact to a staging area"
      }
    }
  }

  post{
    success{
      echo "Deployment was successful"
    }
    failure{
      echo "Error in deployment"
    }
  }
}
