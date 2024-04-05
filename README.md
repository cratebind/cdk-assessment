# CDK Typescript Assessment

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `cdk deploy`      deploy this stack to your default AWS account/region
* `cdk diff`        compare deployed stack with current state
* `cdk synth`       emits the synthesized CloudFormation template

# Problem

You need to setup a AWS CDK Project that contains the following elements:

1. **Create an Amazon S3 Bucket:** The bucket should have public read access disabled to prevent public access to the files it contains.
2. **Create an AWS Lambda Function:** This function should be triggered whenever a new object is uploaded to the S3 bucket. The function should read the content of the uploaded file and log it.
3. **Create an Amazon DynamoDB Table:** The table should have a primary key and at least two other attributes.
4. **Modify the Lambda Function:** After reading and logging the content of the uploaded file, the function should write an item to the DynamoDB table. The item's attributes should be based on the content of the file.

Requirements:
- Use TypeScript as the main programming language.
- Use AWS CDK to define the AWS resources.
- The Lambda function can be written in a language of your choice that is supported by AWS Lambda.
- Include a `README.md` file that explains how to run and test the application.
- Write clean, maintainable code. Consider edge cases and error handling.
- Please add Test cases with Jest or any other Testing framework for the lambda function or other parts you consider important to tests.

##Bonus points: Use RxJS for inside lambda function logic.
