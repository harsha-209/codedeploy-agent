# codedeploy-agent

installation process of codedeployagent

sudo apt-get update

sudo apt-get install python-pip python-pip ruby2.0 wget -y

cd /home/ubuntu

wget https://aws-codedeploy-us-west-2.s3.amazonaws.com/latest/install

chmod +x ./install

sudo ./install auto

sudo service codedeploy-agent status



we have to create two iam roles like
 
 ec2 permission 
  AmazonS3ReadOnlyAccess
AWS managed policy

 AWSCodePipelineCustomActionAccess
 
 ec2 on codedeploy 
 AWSCodeDeployRole
 
 
 and also we have two appspec.yaml file
 
 and shell scripts
 
