# <center>AWS Lambda function trigger event when upload object to AWS S3 then store bucket and object name to DynamoDB</center>

## Overview
In this tutorial, you create a DynamoDB table, a Lambda function and a S3 bucket.  

Then, when you upload an object to S3 bucket, Lambda function will trigger event, run function get bucket and object name and store this to DynamoDB table.

![image](./diagram.png)

## Technical knowledge prerequisites
- AWS IAM
- AWS DynamoDB
- AWS S3
- AWS Lambda
- Python programming

***

Before you use AWS for the first time, you must complete setup steps.

To begin, you must sign up for an AWS account. To sign up, go to https://aws.amazon.com/ and choose Create an AWS Account.

Then you can continue with the rest of the setup tasks in this section.

***

## Tasks:
1. [Create table on DynamoDB](1-DynamoDB/README.md)
2. [Create S3 bucket](2-S3/README.md)
3. [Create Lambda function](3-Lambda/README.md)
4. [Testing the function](4-Testing/README.md)
5. [Clean up your resources](5-Clean-resources/README.md)

***


Next page: [1. Create table on DynamoDB](1-DynamoDB/README.md)

***
Author: Thach Nguyen Van

Github: [https://github.com/thachnv92/](https://github.com/thachnv92/)

Linkedin: [https://www.linkedin.com/in/thachnv92/](https://www.linkedin.com/in/thachnv92/)