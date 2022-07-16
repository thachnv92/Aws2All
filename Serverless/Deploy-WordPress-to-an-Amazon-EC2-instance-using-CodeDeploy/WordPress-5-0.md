# <center>5. Clean up your WordPress application and related resources</center>

# Guide
## 1. CodeDeploy Application
1. Sign in to the AWS Management Console and open the CodeDeploy console at https://console.aws.amazon.com/codedeploy.

2. Choose **`WordPress_App`**.

3. Delete application.

## 2. EC2 Instances
1. Sign in to the AWS Management Console and open the CodeDeploy console at https://console.aws.amazon.com/ec2.

2. Choose **`CodeDeployDemo`** instance.

3. Terminate.

## 3. S3 Bucket
1. Sign in to the AWS Management Console and open the CodeDeploy console at https://console.aws.amazon.com/s3.

2. Choose **`codedeploydemobucket7749`** bucket.

3. Empty.

4. Delete.

## 4. Roles and Policies
1. Sign in to the AWS Management Console and open the CodeDeploy console at https://console.aws.amazon.com/iam.

2. In the navigation pane, choose **Roles**.

3. Search `CodeDeploy` and check in 2 Roles: **`CodeDeployServiceRole`** and **`CodeDeployDemo-EC2-Instance-Profile`**.

4. Delete

5. In the navigation pane, choose **Polices**.

6. Search `CodeDeploy` and check in policy: **`CodeDeployDemo-EC2-Permissions`**.

7. Action > Delete.