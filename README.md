# -AWS-EC2-Terminal-Connect-
This GitHub repository is dedicated to a comprehensive project on connecting to Amazon Web Services (AWS) Elastic Compute Cloud (EC2) instances using a terminal and the AWS Command Line Interface (CLI).

Prerequisites:

1.AWS Account: You should have an active AWS account. If you don't have one, you can sign up at AWS Sign-Up.
2.AWS Access Credentials: Ensure you have your AWS Access Key ID and Secret Access Key. You can obtain these credentials by following these steps:
3.Log in to your AWS Management Console.
4.Open the "IAM" (Identity and Access Management) service.
5.Create a new IAM user or use an existing one.
6.Attach the "AmazonEC2FullAccess" policy or a custom policy with EC2 permissions.
7.Note down the Access Key ID and Secret Access Key for this IAM user.

{Steps to Connect to AWS CLI}

(1) Install AWS CLI: 
If you haven't already, you need to install the AWS CLI on your local machine. Follow these installation instructions based on your operating system:
.Linux:
bash
Copy code
$ sudo apt-get install awscli
.macOS (Homebrew):
bash
Copy code
$ brew install awscli
.Windows:
Download and run the AWS CLI installer from the AWS CLI Download Page.

(2) Configure AWS CLI:
. Open your terminal and configure the AWS CLI with your AWS Access Key ID and Secret Access Key, along with your default region and output format. Replace <YOUR_ACCESS_KEY> and <YOUR_SECRET_KEY> with your actual credentials.
bash
Copy code
$ aws configure
AWS Access Key ID: <YOUR_ACCESS_KEY>
AWS Secret Access Key: <YOUR_SECRET_KEY>
Default region name: <YOUR_REGION>  # e.g., us-east-1
Default output format: json

(3) Verify Your Configuration:
To verify that your configuration is correct, you can run a simple AWS CLI command like aws ec2 describe-instances. If the configuration is accurate, you will receive a JSON response with your EC2 instances (if any exist).
bash
Copy code
$ aws ec2 describe-instances
If successful, you are now connected to AWS CLI, and you can start using it to manage your AWS resources from the terminal.
