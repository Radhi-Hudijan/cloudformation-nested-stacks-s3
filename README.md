# CloudFormation Nested Stacks - S3

This project demonstrates the creation of a CloudFormation nested stack that creates an S3 bucket and uploads an `index.html` file for testing purposes.

## Prerequisites

Before getting started, make sure you have the following:

- AWS account with appropriate permissions
- AWS CLI installed and configured
- Basic knowledge of CloudFormation

## Usage

Follow the steps below to deploy the nested stack:

1. Clone this repository to your local machine.
2. Navigate to the `cloudformation-nested-stacks-s3` directory.
3. Open the `template.yaml` file and review the CloudFormation template.
4. Modify the template as needed to customize the S3 bucket settings.
5. Run the following command to create the nested stack:

```bash
aws cloudformation create-stack --stack-name my-s3-stack --template-body file://template.yaml
```

6. Wait for the stack creation to complete.
7. Once the stack is created, navigate to the AWS S3 console and verify that the bucket has been created.
8. Upload the `index.html` file to the newly created S3 bucket.
9. Access the uploaded `index.html` file using the S3 bucket URL.

## Cleanup

To clean up the resources created by the nested stack, run the following command:

```bash
aws cloudformation delete-stack --stack-name my-s3-stack
```

Please note that this will delete the S3 bucket and all its contents.

For more information, refer to the official AWS CloudFormation documentation.
