pipeline{
    agent any
    tools {
        terraform 'terraform'
    }


    stages{
        stage('Create Infrastructure for the App') {
            steps {
                echo 'Creating Infrastructure for the App on AWS Cloud'
                sh 'terraform init'
                sh 'terraform apply --auto-approve'
            }
        }
    }
}