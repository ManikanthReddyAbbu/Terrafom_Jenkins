pipeline {

agent any

stages {
  stage('Terraform Started') {
    steps {
      sh ' echo "Started..!! " '
    }
  }


  stage('Git Clone') {
    steps {
      sh 'sudo rm -r Terraform_Jenkins/; git clone https://github.com/ManikanthReddyAbbu/Terrafom_Jenkins.git'
    }
  }

  stage('Terraform init') {
    steps {
        sh 'sudo terraform init'
    }
  }

  stage('Terraform Plan') {
    steps {
      sh 'sudo terraform plan'
    }
  }

  /*stage('Terraform apply') {
    steps {
      // One or more steps need to be included within the steps block.
    }
  }*/

  stage('Terraform Ended') {
    steps {
        sh 'echo "The End..!!" '
    }
  }

}

}