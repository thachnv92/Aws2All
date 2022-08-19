# <center>5. Clean up your resources</center>

# Guide
## 1. DynamoDB table
1. Open the DynamoDB console at https://console.aws.amazon.com/dynamodbv2/.

2. In the navigation pane, choose **Tables**, and then check to table which created at [Step 1. Create table on DynamoDB](1-DynamoDB/README.md).
3. Click to **Delete** on top right of screen.
   ![image](./images/clean-01.png)
5. Leave all the defaults and type ```delete``` to text box.
   ![image](./images/clean-02.png)
7. Click to **Delete table**.
   ![image](./images/clean-03.png)
   ![image](./images/clean-04.png)

## 2. S3 Bucket
1. Open the S3 console at https://console.aws.amazon.com/s3/.
   ![image](./images/clean-05.png)
2. Choose bucket which create at [2. Create S3 bucket](2-S3/README.md)
3. Click to **Empty** on top right of screen.
   ![image](./images/clean-06.png)
4. Type ```permanently delete``` to textbox.
   ![image](./images/clean-07.png)
5. Click to **Empty**. Then click to **Exit** on top right of screen after empty bucket successfully to return S3 buckets.
   ![image](./images/clean-08.png)
6. Choose bucket which create at [2. Create S3 bucket](2-S3/README.md)
7. Click to **Delete** on top right of screen.
   ![image](./images/clean-09.png)
8. Type ```bucket name``` to textbox.
   ![image](./images/clean-10.png)
9. Click to **Delete**.
   ![image](./images/clean-11.png)
## 3. Lambda function
1. Open the Lambda console at https://console.aws.amazon.com/lambda/.

2. In the navigation pane, choose **Funtions** which create at [3. Create Lambda function](3-Lambda/README.md)
   ![image](./images/clean-12.png)
3. Check to function and click to **Action** in top right screen, then click **Delete**.
   ![image](./images/clean-13.png)
   ![image](./images/clean-14.png)
4. Type ```delete``` to textbox.
   ![image](./images/clean-15.png)
5. Click to **Delete**.
   ![image](./images/clean-16.png)

## 4. Cloudwatch logs
1. Open the Cloudwatch console at https://console.aws.amazon.com/cloudwatch/.
   ![image](./images/clean-17.png)
2. In the navigation pane, expand **Logs** then click to **Log groups**.
   ![image](./images/clean-18.png)
3. Check to log groups with ```/aws/lambda/<function name>``` and click to **Action** in top right screen, then click **Delete log group(s)**.
   ![image](./images/clean-19.png)
4. Click to **Delete**.
   ![image](./images/clean-20.png)
   ![image](./images/clean-21.png)

***
# <center>End of Guide</center>