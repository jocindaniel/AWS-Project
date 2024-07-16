# AWS-Project
IAM ROLES & USER:
 Create a role for S3 with policies allowing access to S3fullaccess.
 Create a role for Code Deploy allowing code deploy policies.
 Create IAM users with policies allowing full Administration access.
LAUNCH EC2 INSTANCE:
 Launch an EC2 instance as a Production machine in a Linux server and attach the S3 role in it.
 Launch another EC2 instance as a Developer machine in the Linux server.
PRODUCTION MACHINE CONFIGURATION:
 Open production machine CLI via Putty.
 Install and prepare a code-deploy agent on the web server.
DEVELOPER MACHINE CONFIGURATION:
 Open Developer machine CLI via putty.
 Attach IAM User to the developer machine using access keys.
 Create two directories and create an html file that contains the source code of the web application.
 Create yaml file to deploy the source code to the web server automatically.
 Create Code deploy Application and Push the code in Zip format to the S3 bucket from the Developer machine.
CODE DEPLOY:
 Navigate to the AWS code deploy console and create a deployment group.
 Click create deployment which pushes code to the web server.
 The code will be successfully deployed.
CODE PIPELINE:
 Create a code pipeline to enable automatic deployment.
 Both source and deployment succeeded
