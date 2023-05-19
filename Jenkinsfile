pipeline {
    agent any
    tools {
        "org.jenkinsci.plugins.terraform.TerraformInstallation" "terraform"
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