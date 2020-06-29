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
      sh 'sudo git clone https://github.com/ManikanthReddyAbbu/Terrafom_Jenkins.git'
    }
  }

  stage('Terraform init') {
    steps {
        sh 'sudo /home/ubuntu/terraform init ./jenkins'
    }
  }

  stage('Terraform Plan') {
    steps {
      sh 'sudo /home/ubuntu/terraform plan ./jenkins'
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