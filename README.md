# iac_ami
Create AMI from jenkins pipeline.

Create a Jenkins CICD pipeline to create a new Amazon Linux 2 based “Golden Image” AMI. The resulting AMI should have Docker installed. When the AMI is deployed it should start a Docker container of your choice.

1) The Jenkins Environemt is running on EC2 instance (IAM role to admin access. Because of this Jenkins job is able to create AMI 
    a) jenkins job --> pipeline --> packer.json
2) Make sure you have the jenkins URL (http://ec2-3-87-240-26.compute-1.amazonaws.com:8080/github-webhook/ ) given as github webhook 
    Github Repo --> Webhooks --> add the URL (make sure to end that with forward slash)
