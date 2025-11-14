# Lambda_Function
Automatically update AWS Lambda Runtime with Python 🚀

Project Overview
This project automates the process of updating AWS Lambda function runtimes using Python and Boto3. Specifically, I built a script that identifies Lambda functions running on outdated Python runtimes and updates them to newer versions with a single command.

The Problem
AWS Lambda functions often run on older Python runtimes (like Python 3.8), which eventually reach end-of-life and lose AWS support. Manually updating multiple Lambda functions through the AWS Console is time-consuming and error-prone, especially when managing dozens of functions across different regions.

The Solution
I created an automated Python script that:
- Lists all Lambda functions in my AWS account
- Identifies functions running on outdated Python runtimes
- Updates them to a specified Python version (e.g., Python 3.11)
- Provides clear output of all updates performed

Technologies Used

- Python 3.11 - Core programming language
- Boto3 - AWS SDK for Python
- AWS Lambda - Serverless compute service
- AWS IAM - Identity and Access Management for permissions
- AWS CLI - Command-line interface for AWS services

Prerequisites

Before running this project, I have the following:

1. AWS Account with appropriate permissions
2. AWS CLI installed and configured
3. Python 3.x installed on your system
4. Boto3 library installed
5. IAM permissions to list and update Lambda functions


Key Learnings

Throughout this project, I gained hands-on experience with:

1. AWS Lambda - Understanding serverless architecture and function deployment
2. Boto3 SDK - Programmatic interaction with AWS services
3. IAM Roles & Policies - Implementing proper security and access controls
4. Python Scripting - Building automation tools for cloud infrastructure
5. AWS CLI - Managing cloud resources from the command line
6. Error Handling - Dealing with dependency conflicts and environment issues

Challenges Faced & Solutions

Challenge 1: Dependency Conflicts
Problem: Version conflicts between boto3, botocore, and aiobotocore packages.

Solution: pip install --upgrade boto3 botocore aiobotocore s3transfer s3fs

Challenge 2: IAM Role Permissions
Problem: "The role defined for the function cannot be assumed by Lambda" error.
Solution: Created proper trust policy allowing Lambda service to assume the role.

Challenge 3: Module Not Found Errors
Problem: Missing `packaging` module when running the script.

Solution: 
pip install packaging


Resources & References

- [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/)
- [Boto3 Documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)
- [AWS CLI Documentation](https://docs.aws.amazon.com/cli/)
- [Python Packaging Guide](https://packaging.python.org/)

Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

Acknowledgments

- Special thanks to my boss Akhilesh for the comprehensive Training
- AWS documentation and community for extensive resources
- Fellow DevOps Engineers for support and collaboration

---

⭐ If you found this project helpful, please consider giving it a star!

#DevOps #AWS #Lambda #Python #Boto3 #CloudComputing #Automation
