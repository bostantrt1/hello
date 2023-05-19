pipeline{
    agent any
    tools {
        terraform 'terraform'
    }
    
    } 
    stages {
            stage('Terraform'){
            steps {
                dir('jenkins-terraform-pipeline/ec2_pipeline/'){
                    sh "terraform init "
                    sh "terraform apply --auto-approve"
                    sh "echo \$PWD"
                    sh "whoami"
                }
            }
        }
    
}