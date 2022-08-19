# <center>3. Create Lambda function</center>

# Guide

1. Sign in to the AWS Management Console and open the Lambda console at https://console.aws.amazon.com/lambda/. 

    *Note: Choose region same as created S3 bucket in [Step 2. Create S3 bucket](2-S3/README.md).*

2. In the navigation pane, choose **Funtions**, and then choose **Create function**.
   
   ![image](./images/lambda-01.png)

3. On top of page, leave the default with **Author from scratch**.
   
4. In **Basic information** panel, fill information:
   - Function name: `s3-to-dynamodb`.
   - For Runtime, select `Python 3.9` from dropdown.
  
   ![image](./images/lambda-02.png)

5. On the **Advanced settings** panel, leave all the defaults and select **Create function**.

   ![image](./images/lambda-03.png)

6. After function is created. Choose **Configuration**, and then choose **Permissions**.
   
   ![image](./images/lambda-04.png)

7. Under **Resource summary**, review the services and resources that the function can access.
   
   ![image](./images/lambda-05.png)

8. In **Execution role** panel, click to link under Role name.
   
   ![image](./images/lambda-04.png)

9.  In **Permissions**, select **Add permissions** then **Attach policies**.
    
    *Note: Grant least privilege access to your Lambda execution role. Ref [Apply least-privilege permissions](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege).
    However, in this lab, we will pass by this for easier.*
   ![image](./images/lambda-06.png)

10. Filter and check `AmazonDynamoDBFullAccess`, `AmazonS3FullAccess`. Choose **Attach policies**. Close this tab and get back Lambda console.
   ![image](./images/lambda-07.png)
   ![image](./images/lambda-08.png)
   ![image](./images/lambda-09.png)
   ![image](./images/lambda-10.png)

11. On the top, Click to **Add trigger** in **Function overview** panel.
   ![image](./images/lambda-04.png)
   ![image](./images/lambda-11.png)

12. In **Trigger configuration**, type `S3` and select `S3` from dropdown.
    - In **Bucket**, choose bucket created in [Step 2. Create S3 bucket](2-S3/README.md).
    - In **Event type**, select `PUT` from dropdown. Leave all the defaults and check to **Recursive invocation**. Select **Add**.

    ![image](./images/lambda-12.png)
    ![image](./images/lambda-13.png)

13. Choose **Code**, and then update code in lambda_function.
   ![image](./images/lambda-14.png)

14. Click to **Deploy** after update code.

   Ref [lambda_function.py](functions/lambda_function.py)
    
***
Next page: [4. Testing the function](../4-Testing/README.md)